# ransack
A simple and flexible package manager

# What is ransack?
Ransack, named after the Transformers Cybertron character, is a source-based package management system that is suitable for anyone, especially those who're building their own distribution, or just want a package management system whose packages could be hosted anywhere easily. It's so easy that one would only need a simple online directory, or even a GitHub repository.

# How to use ransack?
Ransack consists of a few arguments. These are;

--install/-i to install a package (it triggers the {packagename} script)

--uninstall/-r to remove a package (needs a {packagename}-uninstall script, so devs, please make one.)

--setup/-s to establish the /sourcescript and /sourcescript/AppImages directories (needed for downloading scripts using --update/-u argument)

--update/-u is to update the scripts (supposedly) by cleaning the /sourcescript directory (make sure to backup your AppImages, since they'll be gone as well! BOOM! GONE!)

--appimage/-a is to download an AppImage hosted on a repo (not AppImageHub).

--flatpak/-F is to download a Flatpak package.

# Great! Now I know how to use it, how can I make packages for ransack?

It's great that you've asked this question. You can make packages using the "example" file, which is an example file on how to make a package. It also shows a guideline to create a package.

# Dependencies
- wget
- AppImageCrafters/appimage-cli-tool
