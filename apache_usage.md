APACHE USAGE INSTRUCTIONS
========================

Contents
--------

- [Configuration Files](#configuration-files)

# Configuration files
## sites-enabled and sites-available directories

The difference is that virtual sites listed in the `/etc/apache2/sites-enabled/` directory are served by apache.
In the `/etc/apache2/sites-available` directory there are the virtual sites that exist on your server but people can't access them because they are not enabled yet.

You should edit files only in sites-available directory.
Do never edit files inside the sites-enabled directory, otherwise you can have problems if your editor runs out of memory or, for any reason.
That will prevent Apache or NGINX to start.

[Source](https://stackoverflow.com/questions/21812360/what-is-the-difference-between-sites-enabled-and-sites-available-directory)
