- create project using laravel
  + laravel new projectName => get version 5.4
- create project using composer
  + composer create-project laravel/laravel {directory} 4.2 --prefer-dist =>get version 4.2

- run open project
  + php artisan serve

- create controller
  + php artisan make:controller ControllerName

- create model
  + php artisan make:model ModelName

- php artisan make:
  	make:auth            Scaffold basic login and registration views and routes
  	make:command         Create a new Artisan command
  	make:controller      Create a new controller class
  	make:event           Create a new event class
  	make:job             Create a new job class
  	make:listener        Create a new event listener class
  	make:mail            Create a new email class
  	make:middleware      Create a new middleware class
  	make:migration       Create a new migration file
  	make:model           Create a new Eloquent model class
  	make:notification    Create a new notification class
  	make:policy          Create a new policy class
  	make:provider        Create a new service provider class
  	make:request         Create a new form request class
  	make:seeder          Create a new seeder class
  	make:test            Create a new test class migrate
  	migrate:install      Create the migration repository
  	migrate:refresh      Reset and re-run all migrations
  	migrate:reset        Rollback all database migrations
  	migrate:rollback     Rollback the last database migration
  	migrate:status       Show the status of each migration

-  Create a new controller class
   + php artisan help make:controller
-  Create Login / register
   + php artisan make:auth

Usage:
  make:controller [options] [--] <name>

Arguments:
  name                  The name of the class

Options:
      --resource        Generate a resource controller class.
  -h, --help            Display this help message
  -q, --quiet           Do not output any message
  -V, --version         Display this application version
      --ansi            Force ANSI output
      --no-ansi         Disable ANSI output
  -n, --no-interaction  Do not ask any interactive question
      --env[=ENV]       The environment the command should run under.
  -v|vv|vvv, --verbose  Increase the verbosity of messages: 1 for normal output, 2 for more verbose output and 3 for debug


- create schema tabel
  + php artisan make:migration create_user_table --create=tbl_users
  + can add more fiel and update 

- add table schema to phpmyadmin
  + php artisan make:migrate

- have to create driver
  + touch database/database.sqlite

- create model 
  + php artisan make:model ModelName --migration

- clear cach / view route list
  + php artisan cache:clear
  + php artisan route:cache
  + php artisan route:clear
  + php artisan route:list

=============================convert MKV to MP4==============================
So to convert an MKV file to MP4:

1.  Run "VLC media player".
2.  From main menu select "Media" > "Convert / Save...".
3.  On "File" tab, click "Add..." button.
4.  Choose you MKV file. After that, it should be added to the list. (Alternatively, you can drag&drop a file into the list.)
5.  Click "Convert/Save" button.
6.  Select Profile: "Video - H.264 + MP3 (MP4)".
7.  Click on the icon button that has hint: "Edit selected profile".
8.  On "Encapsulation" tab, leave "MP4/MOV" selected.
9.  On "Video codec" tab, check both "Video" and "Keep original video track".
10. On "Audio codec" tab, similarly select both "Audio" and "Keep original audio track".
11. Click "Save" button.
12. In "Destination" selection, click "Browse" button to select directory and file name for you destination MP4 file.
13. Click "Start" button.
14. Observe progress bar in the main window as file is converted.
15. After that, my VLC (version 2.2.1) seems to hang in an infinite loop so I have to kill it using system "Task Manager", but it doesn't matter - the destination file is already created.