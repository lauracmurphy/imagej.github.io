---
autogenerated: true
title: TEM suite
breadcrumb: TEM suite
layout: page
author: test author
categories: 
description: test description
---

This is a suite of useful imageJ plugins that are designed for analysis of images and diffraction patterns taken on a Transmission Electron Microscope (TEM). Included in the suite are:

1.  [calc dSpace](calc_dSpace "wikilink") is a simple way to find interplanar spacing values in imageJ.
2.  [get dSpace](get_dSpace "wikilink") is a more accurate and advanced way of finding d-spacing.
3.  [pub Montage](pub_Montage "wikilink") is a high quality montaging plugin designed for figure submission to a peer review journal.
4.  [get Meta](get_Meta "wikilink") extracts the metadata from all the DM3 files in the directory and saves them to a text file within that directory.

## Getting Started

The following are ways of installing this suite of plugins. The first way is the easiest and fastest method, but the second way offers more freedom.

### Installation via FIJI updater

The easiest way to install the TEM suite of plugins is to use the FIJI updater:

1.  Download and install [FIJI](https://fiji.sc/)
2.  Start the updater with *Help* \> *Update*
3.  Click the *Manage update sites* button in the *ImageJ Updater Window*
4.  In the *Manage update sites window* scroll down to the **TEM suite** entry and check the box in the left hand column
5.  Close the *Manage Update Sites* window and click the *Apply Changes* button on the *ImageJ Updater Window*
6.  Restart ImageJ

This will install the plugins in a plugin/sripts/TEM folder, which has the advantage of creating it's own menu item in ImageJ, so you don't have to go hunting for it in the massive Plugins menu.

![Menu.jpg](/images/pages/Menu.jpg "Menu.jpg")

### Manual Installation

If you want to just use one of the plugins or you want to place them in a different location, follow these steps:

1.  The text of these scripts can be viewed on the [update site](http://sites.imagej.net/Makoten/plugins/Scripts/TEM/)
2.  Click on the plugin you want (make sure it is the most recent release)
3.  Copy the text of the desired plugin and paste it into a blank text file
4.  Save it with the extension .ijm in the desired location within your imageJ application
5.  Go to *Help* =\> *Refresh Menus*
6.  Restart ImageJ