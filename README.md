# Lumin OS App Guide

So, you want to make an app for Lumin OS, right?

## Starting

First, download the Example ZIP from the releases, then extract it into a folder.

Edit the config.cfg contents. Only `APP_NAME`, `APP_ID`, `AUTHOR`, `SYSTEM_APP` and `CATEGORY` matter.

## Coding

Now, go to the bin folder. You will find app.cmd.

Remove everything except `@echo off` (prevents paths from appearing), `title` (sets the window title) and `chcp` (sets text encoding to UTF-8, this is necessary to avoid garbage characters when using extended ASCII characters)

Now, code your app. Use exit /b to go back to desktop. Use >nul to not show output. Combine >nul with a space and 2>&1 to redirect errors to normal output (hides errors too). You can also modify title.

## Preparing your app for installing

Flat-zip your app by selecting everything on the root of your app (Ctrl+A), then right clicking and compressing into a ZIP file using the  Windows default ZIP compresser.

Rename the ZIP extension from `.zip` to `.lapp`. It is the default extension for Lumin OS apps.

Rename the `.lapp` file to whatever you want. **Do NOT modify the file extension.**

Then move the `.lapp` to the root of your USB0 (obtained from Lumin OS Unlocker).

## Installing the app

Boot Lumin OS, then go to the App Sideloader. Your app package should appear. Select the package.

When it finishes installing, quit the App Sideloader and go to the App Drawer.

There you will find your app. Select it.

And voila! You just finished installing your first app.

## App Repository

I will soon be releasing an App Repository. Stay tuned.
