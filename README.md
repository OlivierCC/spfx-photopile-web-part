## Photopile Web Part

The photopile-web-part project is a SharePoint web part built using the SharePoint Framework (SPFx) in the preview version.
This project implements the great [Photopile.Js](https://github.com/bigbhowell/Photopile-JS) created by Brian W. Howell
(a popular jquery script) as a client side web part for SharePoint.

With this Web Part, you can display the photos contained in a SharePoint Pictures Library as a cool image gallery that
simulates a pile of photos scattered about on a surface. Thumbnail clicks remove photos from the pile,
(enlarging them as if being picked up by the user), and once in  view a secondary click returns the photo to the pile.

![Photpile Web Part displayed in SharePoint Workbench](./assets/photopile-overview.gif)

## Run this web part in the SharePoint workbench

```bash
git clone the repo
npm i
tsd install
gulp serve
```

If you need more information about to develop SharePoint Framework client side web part, deploy and test it on your workbench
station, you can consult the following tutorial: https://github.com/SharePoint/sp-dev-docs/wiki/Setup-SharePoint-Tenant

## Features

This web part uses React, Office UI Fabric, JQuery, JQuery UI and Photopile.js. This web part is available in English (en-us)
and French (fr-fr). You can use this web part with SharePoint Online (Office 365) or SharePoint Server 2016.

It is able to:
* List Picture Libs contained in the current SharePoint web site
* List all the pictures in the selected List
* Render the pics as a cool photopile
* Personalize the layout thanks to editable settings

If you are a SharePoint web developer, you can be interested by the following code patterns :
* Include JQuery and external framework in your solution
* Implement rich web part properties panel with controls like DropDown, Sliders, Toggle, etc.
* Load dynamic data from SharePoint as web part properties
* Load dynamic data from SharePoint REST Services, as lists or items
* Implement mock system to test your solution in the local workbench or on a SharePoint site
* Include Office UI Fabric controls in your project
* Render content with React
* Etc.

## How to use it

By compiling this code on a configured workstation, you can test this web part on your local SharePoint workbench
or on a developer site. Please follow the tutorials in the SPFx tutorial to know the process : https://github.com/SharePoint/sp-dev-docs/wiki/Setup-SharePoint-Tenant

You can also test this web part directly as SharePoint App (spapp package).

**Please note that the SharePoint Framework (SPFx) is currently in public preview, so this kind of client side web part are not supported in a production site.**

To test the web part on a SharePoint site, follow this steps :

1. Download the [photopile-web-part.spapp](./sharepoint/photopile-web-part.spapp) on your desktop
2. Connect on your tenant with a SharePoint Online administor account, and go in the App Catalog web site
3. Insert the web part in your tenant App catalog (drag & drop the photopile-web-part.spapp in the "App for SharePoint" list
