# WARNING: IT'S NOT AFFILIATED WITH ANY OTHER PROJECT THAT IS NAMED RANSACK!
# ransack
A simple and flexible package manager

# What is ransack?
Ransack, named after the Transformers Cybertron character, is both a binary-based and a source-based package management system that is suitable for anyone, especially those who're building their own distribution, or just want a package management system whose packages could be hosted anywhere easily. It's so easy that one would only need a simple online directory, or even a GitHub repository.

# How to use ransack?
Ransack consists of a few arguments. These are;

--install/-i to install a package (it triggers the {packagename} script)

--uninstall/-r to remove a package (needs a {packagename}-uninstall script, so devs, please make one.)

--setup/-s to establish the /sourcescript and /sourcescript/AppImages directories (needed for downloading scripts using --update/-u argument)

--update/-u is to update the scripts (supposedly) by moving the files from /sourcescript directory to /sourcescript/old (make sure to backup your AppImages, since they'll be moved to the following directory as well! BOOM! GONE!)

--appimage/-a is to download an AppImage hosted on a website that is mentioned in the script.

--flatpak/-F is to download a Flatpak package.

--source-install: installs a package using a download script (category/package, e.g. app-emulation/cemu), but the package is compiled on your machine instead of using a binary.

# Great! Now I know how to use it, how can I make packages for ransack?

It's great that you've asked this question. You can make packages using the "template" file, which is an example file on how to make a package. It also shows a guideline to create a package. Or alternatively, you can use "example-flatpak" and "example-appimage" files to download packages that are using those package formats.

# Dependencies
- wget
- <a href="https://github.com/AppImageCrafters/appimage-cli-tool"> AppImage CLI Tool (only for installing AppImages)</a>

# Future
- Add binary support
- replace wget with wget2 or aria2c