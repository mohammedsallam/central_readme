## To install project follow next steps.
    
   1- Install composer.packages.
    
    You need to install Compser first on your machine, you can download and install Composer from [#Here](https://getcomposer.org/doc/00-intro.md)
    
    composer install 
    
   2- Create .env file.
    
    cp .env.example .env 
    
   3- Make your DB, and set the configuration in the env file.
    
   4- Generate key for application.
    
    php artisan key:generate 
    
   5- Migrate Database.
    
    php artisan migrate 
        
   6- Seed database.
   
    php artisan db:seed
    
    
   7- Now you can browse the admin from `URL/admin` using this account
   
   `email: super@admin.com`
   
   `password: 123456`



