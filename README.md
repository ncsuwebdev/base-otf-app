#Base OT Framework App#

This the a skeleton app to allow a user to quickly start creating an app based on OT Framework (http://github.com/ncsuwebdev/otframework).

You can install this via composer (http://getcomposer.org) by:

   ``` sh
   $ composer.phar create-project ncsuwebdev/base-otf-app [install directory] [version]
   ```
**NOTE! The install directory should not exist before running the script**


Once you create the project, you will need to do a few steps to get going:

* Copy /application/configs/application.default.ini to /application/configs/application.ini
* Create a database and put the credentials in the development section in application.ini
* Run the database migration script to install the db.  
   ``` sh
   $ php otutils/migrate.php -c latest -e development
   ```

* Go to http://[path-you-installed-this] and you can log in with admin/admin credentials