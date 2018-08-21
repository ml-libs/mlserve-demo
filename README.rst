mlserve-demo
============
Demo project for **mlserve** deployed on heroku.


* https://young-ridge-56019.herokuapp.com

Deployement
-----------


    $ pip install git+https://github.com/jettify/mlserve.git
    $ heroku create
    $ git push heroku master
    $ heroku logs --tail
    $ heroku open


Purge caches
------------

https://help.heroku.com/18PI5RSY/how-do-i-clear-the-build-cache
    $ heroku plugins:install heroku-repo
    $ heroku repo:purge_cache -a appname
    $ git commit --allow-empty -m "Purge cache"
    $ git push heroku master
