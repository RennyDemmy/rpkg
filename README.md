# ransack
A simple and flexible package manager

# What is ransack?
Ransack, named after the Transformers Cybertron character, is a source-based package management system that is suitable for anyone, especially those who're building their own distribution, or just want a package management system whose packages could be hosted anywhere easily. It's so easy that one would only need a simple online directory, or even a GitHub repository.

# How to use ransack?
Ransack consists of a few arguments. These are;
--install/-i to install a package (it triggers the {packagename} script)
--uninstall/-r to remove a package (needs a {packagename}-uninstall script, so devs, please make one.)
--setup/-s to establish the /sourcescript directory (needed for downloading scripts using --update/-u argument)
--update/-u is to update the scripts

