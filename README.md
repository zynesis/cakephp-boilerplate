CakePHP Boilerplate
========

CakePHP Boilerplate for Zynesis projects.

Loaded with the following goodies:

1. Composer
1. CakePHP 2.x (loaded [via Composer](http://ceeram.github.io/blog/2013/06/18/adding-cakephp-as-composer-package/))

CakePHP plugins:

1. [ClearCache](https://github.com/ceeram/clear_cache)
1. [DebugKit](https://github.com/cakephp/debug_kit)
1. [TwitterBootstrapHelper](https://github.com/zynesis/twitter-bootstrap-helper) (Zynesis fork)

Other vendor packages:

1. [Bootstrap 2.3](https://github.com/twbs/bootstrap)

Set up
--------
1. Install Composer packages

   If you do not yet have Composer installed on your system, follow the guide here on [how to install Composer](http://getcomposer.org/doc/00-intro.md#globally).

   ```bash
   composer install
   ```

1. Make these dirs and files writable by web server:

   ```bash
   chmod -R 777 tmp
   ```

1. Set up database and other local settings

   ```bash
   cp Config/database.php.default Config/database.php
   cp Config/local.php.default Config/local.php
   ```

   Edit `database.php` and `local.php` with your local settings

1. Point `DocumentRoot` _(or equivalent)_ of your web server to `webroot/`. Enjoy!


Notes
----
1. Model recursiveness is set to -1 by default.

1. To clear cache, simply `Console/cake ClearCache.clear_cache`.

Credits
----
Loading of CakePHP via Composer is made possible thanks to [Ceeram's idea](http://ceeram.github.io/blog/2013/06/18/adding-cakephp-as-composer-package/).
