This the a skeleton app to allow a user to quickly start creating an app based on OT Framework (http://github.com/ncsuwebdev/otframework).

You can install this via composer (http://getcomposer.org) by:

:$ composer.phar create-project ncsuwebdev/base-otf-app [install directory] [version]

Once you create the project, you will need to do a few steps to get going:

1)  Copy /application/configs/application.default.ini to /application/configs/application.ini

2)  Create a database and put the credentials in the appropriate section in application.ini

3)  Run the database migration script to install the db.  

   :$ php otutils/migrate.php -c latest -e development

4)  Go to http://[path-you-installed-this] and you can log in with admin/admin credentials
