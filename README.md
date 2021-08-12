How to use
------------
I recommend to do the following instructions in `centos:7` container with a mounted volume.


Clone Repositories
------------
### Remove default repos

    $ rm -f /etc/yum.repos.d/*

    ## Remove all yum cached data
    $ yum clean all

### Add target repos

    $ mv sample.repo /etc/yum.repos.d/sample.repo

### Clone repos
    ## Generate the metadata cache
    $ yum makecache

    ## Check if the repositories are configured correctly
    $ yum repolist

    ## Clone repos
    $ reposync -p /etc/yum.repos.d/


Serving your own repositories
------------

    # TODO



Found mistakes?
------------
Feel free to make a pull request if you find any mistake or better way to make the explanation more clear.

Contact me
------------
Contact me through
[email](mailto:muller79924@gmail.com)
in english or chinese.
