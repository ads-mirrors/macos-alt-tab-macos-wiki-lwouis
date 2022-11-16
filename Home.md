# AltTab - Usage and Configuration

**AltTab** brings the power of Windows’s "alt-tab" window switcher to macOS.

Official website - features, installation, etc.: https://alt-tab-macos.netlify.app/  
Bug reports and discussion of issues: https://github.com/lwouis/alt-tab-macos/issues  
Wiki: https://github.com/lwouis/alt-tab-macos/wiki

## Usage

AltTab works similarly to Apple's built-in `command-tab` application switcher, but for specific windows. It is activated by holding down the `alt` (also known as `option`) key, and pressing `tab`. By default, it shows a scrollable list of thumbnails for all open windows. While continuing to hold down `alt`, repeatedly pressing `tab` cycles forward through the thumbnails, and pressing the `shift` key cycles backwards. The arrow keys, or hovering the mouse pointer over a thumbnail, can also be used. Releasing `alt`, pressing the `space` bar, or clicking on a thumbnail, displays the selected window. Pressing `esc` cancels. The display of thumbnails can be restricted to only the active application, by using `alt` with `` ` `` (the "backtick" key) instead of `tab`.

The thumbnail list is rearranged in "most recently used order", so that quickly pressing `alt-tab` will switch back and forth between the two most recently used windows. 

Hovering the mouse pointer over a thumbnail shows clickable controls to quit the app, or close/minimize/maximize the window. The keyboard shorcuts `Q`, `W`, `M` can also be used, and `H` can be used to hide the application. The thumbnails support drag and drop of items from other applications.

AltTab offers extensive configuration options in the Preferences, found in the menu under the AltTab icon in the Mac menu bar. See below for details.

### A note about Stage Manager

Apple's Stage Manager feature, introduced in macOS 13 "Ventura", impacts users of AltTab. The window thumbnails displayed in AltTab may appear 
low-resolution and skewed or tilted, similar to the application and window thumbnails of Stage Manager. Stage Manager can be turned off in the Control Center.

Alternatives include hiding the display of AltTab's thumbnails in its settings, and showing only the window titles. Another option is turning off the display of the Stage Manager thumbnails, allowing them to auto-display when hovering the mouse pointer over the area. To do this, in System Settings > Desktop & Dock > Stage Manager > Customize, uncheck "Recent applications". This will result in normal thumbnails in AltTab. However, you may find that the thumbnails are blank if the window has not been displayed yet, and other problems. See [issue #1731](https://github.com/lwouis/alt-tab-macos/issues/1731) for discussion and details.

## Configuration

Choose "Preferences" in the menu under the AltTab icon in the Mac menu bar, to access the settings.

### General

Choose whether to start AltTab automatically at login, and which icon to use in the menu bar.

### Controls

AltTab can have up to five different shortcuts. The first two are pre-configured for `alt-tab` and `` `-tab ``. You can change or configure the shortcut keys, which windows/spaces/screens are shown, etc.

### Appearance

The appearance of the thumbnails list can be customized.

Theme: choose a Mac (round corners etc.) or Windows-like (square corners etc.) theme.

Align windows: choose whether thumbnails are centered or aligned left inside the list window. It is not currently possible to change the vertical alignment of the list window.

Max width/height on screen: The maximum size of the thumbnails list window, as a percentage of the screen size. This will also interact with the size of the thumbnails. The 100% width setting still has some margins.

Hide window thumbnails: don't show window thumbnails, only application icons and window titles.

Rows of thumbnails: the maximum number of rows to display without scrolling. This may also interact with the size of the thumbnails, and produce unexpected results.

Window min width in row: the minimum width of a thumbnail, as a percentage of the width of the thumbnail list display. Thumbnails for narrow windows will be padded with blank space.

Window max width in row: the maximum width of a thumbnail, as a percentage of the width of the thumbnail list display. Wide windows will be shrunk to fit within the thumbnail. The slider's lower limit, and possibly its value, changes based on the minimum width set above: the maximum width cannot be set lower than the minimum width.

Window app icon size: the size in pixels of the icon identifying the application that the window belongs to.

Window title font size: the height in pixels of the window title in each thumbnail.

Window title truncation: where the title is cut off, if it doesn't fit within the thumbnail.

Show on: where to show the thumbnail display: on the active screen, the screen where the mouse pointer is, or the screen where the main menu bar is.

Apparition delay: delay before showing the thumbnail display. Useful if you find the display flashing on, when you only mean to quickly switch between the most recent windows, without activating the display.

Fade out animation:

Hide Space number labels:

Hide status icons:

Show standard tabs as windows: applications that use macOS tabs for multiple windows or documents will have separate thumbnails for each. This does not work for Safari or other browser tabs, or any other application that manages its own tabs.

Hide colored circles on mouse hover: do not display the thumbnails' buttons for quit, close, minimize, and zoom.

Hide app badges: do not display notification "badges" on the application icons, that can be seen in the Dock, for example, the count of unread messages in Mail.

Hide apps with no open windows: by default, a thumbnail is shown allowing a new window to be opened. This setting disables that. See "Blacklists" below to always hide a specific application.

### Policies

Settings for application updates and crash reports.

### Blacklists

Rules for dealing with specific applications or processes, such as hiding them from the thumbnails list or ignoring shortcuts for them. Useful if an application does not behave as desired.

### About

Version and license information, and a link to send feedback.

### Acknowledgements

Acknowledgements for contributors and third-party libraries.
