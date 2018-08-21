mlserve-demo
============
Demo project for **mlserve** (https://github.com/jettify/mlserve) deployed on heroku.


* https://young-ridge-56019.herokuapp.com

Deployement
-----------
Execute following commands::

    $ pip install git+https://github.com/jettify/mlserve.git
    $ heroku create
    $ git push heroku master
    $ heroku logs --tail
    $ heroku open


Purge caches
------------
Sometimes it is usevull to purge pip caches to force app to use new library::

    $ heroku plugins:install heroku-repo
    $ heroku repo:purge_cache -a appname
    $ git commit --allow-empty -m "Purge cache"
    $ git push heroku master


https://help.heroku.com/18PI5RSY/how-do-i-clear-the-build-cache
