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

This web part uses React, Office UI Fabric, JQuery, JQuery UI and Photopile.js.

It is able to:
* List Picture Libs contained in the current SharePoint web site
* List all the pictures in the selected List
* Render the pics as a cool photopile
* Personalize the layout thanks to editable settings

## How to use it


