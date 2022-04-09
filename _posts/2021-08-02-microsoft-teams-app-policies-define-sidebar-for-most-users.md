---
title: "Microsoft Teams: App Policies"
date: "2021-08-02T09:05:00-04:00"
author: "Ryan Robinson"
layout: post
permalink: /microsoft-365/microsoft-teams/microsoft-teams-app-policies-define-sidebar-for-most-users/
image: 
  src: /assets/img/logo/Teams.png
  width: 300
  height: 300
  alt: "Microsoft Teams logo: stylized purple T"
categories:
  - "Microsoft 365"
  - "Microsoft Teams"
tags:
  - MS-700
---

Suppose you want to lock the sidebar in Teams for some users to ensure that they don’t have different experiences, which can help with providing support and documentation as well as make sure nobody accidentally loses their easy access to the app they want to use. But you don’t want to lock all users; there are some like your IT department that might need some freedom to use their Teams differently.

This can be done with an app setup policy in the Microsoft Teams admin centre.

For this example, I’ll set the taskbar to contain:

- Activity
- Chat
- Teams
- Calendar
- Files

I’ve removed the Calls app from the default, since I don’t use Teams for a phone system and the Calls app is somewhat underwhelming without that.

I’ll also default install Tasks by Planner and To Do, but not force it on the taskbar.

## Edit the global policy

Start out in the Teams Admin Centre, at <https://admin.teams.microsoft.com>.

In the navigation, go to Teams Apps -&gt; Setup Policies.

Click on the Global (Org-wide default) policy. Change a few settings here:

- Flip the toggle for “Allow user pinning” off.
- Under “Installed apps,” click on “Add apps,” search for Tasks by Planner and To Do, and add
- Under “Pinned apps,” select beside Calls and then click the Remove button

Click Save when done.

![Policy editing screen with sections for general settings, installed apps, and pinned apps](/assets/img/2021/07/Global-policy-changes.png)
_Screenshot of Teams admin with the changes described above_

When a user signs in, they’ll now have this as their default app bar:

![](/assets/img/2021/07/Global-policy-with-no-calls-app.png)
_Sidebar, with no Calls app_

Furthermore, if they try to pin any other apps to their sidebar, they will not see the “pin” option anymore.

We now have a default locked sidebar for all users.

## Create a custom policy

The next step is that we want there to be an exception for one user. Back on the setup policies screen in the Teams Admin Centre, I’ll add a new policy.

On the screen to edit the policy. This time I’ll:

- Set the toggle for “allow user pinning” to On
- Leave everything else the same as the default

Click Save when done.

![Policy editing screen with general settings, installed apps, and pinned apps](/assets/img/2021/07/Freedom-policy.png)
_Screenshot of the editing screen for the policy that does not lock the taskbar_

## Apply the custom policy

Now that the policy is created, you need to assign it to a user. Select the policy, then click the Manage user button. It will pop out a sidebar with a people search box to look up your users that you want to apply the policy to. Select Add for that user. Once you’ve added everybody, click Apply.

![Manager users for the "Freedom" policy, adding the user "Ryan Robinson"](/assets/img/2021/08/Add-user-to-Teams-app-policy.png)
_Sidebar for adding users to a policy_

That’s it. You’ve successfully modified the default policy a bit more strict but then allowed an exception for a smaller group of users.
