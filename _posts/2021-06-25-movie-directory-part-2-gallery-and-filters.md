---
title: "Movie Directory Part 2: Gallery and Filters"
date: "2021-06-25T14:03:00-04:00"
author: "Ryan Robinson"
layout: post
permalink: /microsoft-365/power-apps/movie-directory-part-2-gallery-and-filters/
image: 
  src: /assets/img/logo/Power-Apps.jpg
  width: 300
  height: 300
  alt: "Power Apps logo"
categories:
  - "Power Apps"
tags:
  - "Movie Directory"
---

In [Movie Directory Part 1](/microsoft-365/power-apps/movie-directory-part-1-the-data/), I described what I was aiming to achieve with this personal project, as well as the Dataverse structure.

In this post, I’ll describe at a high level the design of the Power App and the gallery view and filters. Most of it I’ll keep at a high-level, not step-by-step, as I used a lot of the out-of-the-box functionality.

## Screens

There are four screens involved in the app:

- Gallery view that shows all of the movies, with the cover art behind the title, year, and last time we watched it
- Filters screen that allows you to specify filters that apply on the gallery view
- View details screen of a single movie
- Edit details screen of a single movie, including a new movie

## All Movies

![](/assets/img/2021/06/Gallery-view.png)
_Gallery view. We own all the Alien movies_

The majority of this screen is a Gallery component, with some minor changes to show exact details I wanted to show. The biggest change is incorporating the filters from the filters screen, which required this in the OnVisible field to handle whether there are filters set or not:

```
Set(MoviesFilter1,If(!IsBlank(varWatchlist)&&varWatchlist<>"None",Filter(Movies,Text(Watchlist)=varWatchlist),Movies));
Set(MoviesFilter2,If(!IsBlank(varOwned),Filter(MoviesFilter1,varOwned in Owned),MoviesFilter1));
Set(MoviesFilter3,If(!IsBlank(varLastWatched),Filter(MoviesFilter2,'Last Watched'>=varLastWatched||IsBlank('Last Watched')),MoviesFilter2));
```

And this in the Items field to only show those with the right filters:

```
SortByColumns(
    If(IsBlank(TextSearchBox1.Text),MoviesFilter3, Filter(Movies,TextSearchBox1.Text in Text(Name))),
        "crfa4_name", 
        If(SortDescending1, SortOrder.Descending, SortOrder.Ascending)
    )
```

The OnSelect field of the Overlay on the gallery has this, to navigate to viewing that specific movie:

```
Navigate(ViewMovieDetails,ScreenTransition.Fade)
```

Setting the background image was a bit simpler, putting this into the Image field of the Image component in the Gallery:

```
ThisItem.Cover.Full
```

Another minor tweak included adding the Filters icon, which navigates to the filters screen with this formula in the OnSelect:

```
Navigate(MovieFilters)
```

## Filters

![](/assets/img/2021/06/Filters.png)
_Filters screen_

The filters screen is nothing flashy, but functional. The watchlist field is a simple dropdown, where the items field comes from the Dataverse tables:

```
Choices(Movies.Watchlist)
```

Similar for the Owned Platform field:

```
Choices(Movies.Owned)
```

Hide Movies Watched Since is a standard date picker field, but those are hard to blank out if you had that set and then wanted to turn it off, so I had to add an accompanying button with this OnSelect value:

```
Reset(LastWatchedFilter)
```

The hardest part is the Save button, which needed to update the filter variables and navigate back to the gallery view, so this goes into the OnSelect for that button:

```
Set(varWatchlist,WatchlistFilter.SelectedText.Value);
Set(varOwned,OwnedFilter.Selected.Value);
Set(varLastWatched,LastWatchedFilter.SelectedDate);
Navigate(AllMovies)
```

That’s it for the gallery view and filtering. The next post in this series will describe viewing and editing of a single movie.
