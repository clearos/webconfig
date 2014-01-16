ClearOS Webconfig
=================

ClearOS Webconfig Super-project.

Cloning
-------

To clone the entire Webconfig super-project you must enable recursive mode, for example:

    # git clone --recursive git@github.com:clearos/webconfig.git

App Submodules
--------------

To add a new app submodule, run the following from the webconfig top-level directory.  Example:

    # git submodule add git@github.com:dsokoloski/clearos-ibvpn.git apps/ibvpn
    # git commit -a
    # git push

To update all submodule projects to their master branches, run the following from the webconfig top-level directory:

    # git submodule foreach git pull origin master
    # git commit -a
    # git push

To rename an app submodule's Git URI, edit .gitmodules and then run the following from the top-level directory:

    # vi .gitmodules
    # git submodule sync
    # git commit -a
    # git push

