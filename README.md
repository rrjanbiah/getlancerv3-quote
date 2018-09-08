Getlancer-Quote is an Open Source service marketplace script which enables the entrepreneur to run a successful Thumbtack similar website of their own.

![Thumbtack Clone Website](https://user-images.githubusercontent.com/43058084/45251565-e7fd3500-b365-11e8-8e83-34f2983d6f67.png)

**How it works**

[Thumbtack clone](https://www.agriya.com/products/thumbtack-clone) script defines two communities, service provider and the others who wants the service to get it done. Users can post their request by means of job and that will be notified to all the service professionals who are expertise in the particular area of interest. So the service pro can send quote to the defined task therefore you can get multiple quotes from several service pro as well. 

Once you finalize with the particular service pro, then you can communicate with them and get your job done. Once the job completes, Service pro and the others can review each other.

![Thumbtack Clone](https://user-images.githubusercontent.com/43058084/45252743-aecec000-b379-11e8-8e42-aa13636f3c4b.png)

**What is Special in our Agriya's Thumbtack Clone Script**

  Besides the mushrooming features in our competitve service marketplace script, there are certain key features which we represent as a
  functional USP's of this Thumbtack clone product.
  
**Geo Location Based Listing**

  Ease of finding your local service provider with our Geo-based listing functionality with crystal clear accuracy.
  
**Intuitive Category Management**

  Whatever be your business model is, we made our script with dynamic form builder whereby you can create any service to the extent      without having any difficulties.

**Dual Sign up**

Every coin has two sides. Similarly, one can be either Service pro or an user based on their instance. Through a single access details, they can act as both the roles.

**Interoperability**

Tired of updating the website whenever the new trend unveils? Agriya's Thumbtack clone script is power-packed with Front and Back approach. So you can have an absolute freedom to customize the website easily with oyur intended data metrics.

**AI Enabled Script**

Most of the functionalities are automated as it feels the current stats and takes you to the intended space where you can obtain your needed data as well. We indulged with bot mechanism with the script to make it more friendly with the search engines.


Installation Steps
------------------
# Server Requirements

    ** PHP Version - PHP >= 5.6
        * Extensions
            GD Version - 2.x+
            PCRE Version - 7.x+
            cURL version - 7.x+
            json version - 1.x+
            OpenSSL
            PDO PHP Extension
            mbstring
        * php.ini settings
            max_execution_time - 180 (not mandatory)
            max_input_time - 6000 (not mandatory)
            memory_limit - 128M (at least 32M)
            safe_mode - off
            open_basedir - No Value
            display_error = On
            magic_quotes_gpc = Off
    ** postgres sql : 9.4
    ** ngnix server
        Nodejs
        Composer
        Bower
        Grunt
    Recommended Linux distributions: Centos / Ubuntu / RedHat

# Server Side

### Composer Updation

To Update the Composer, please run the below command in your Project Path.  

* Path - server/php/Slim

        composer install
    
* The above Updation doesn't work to you, need to install Composer, please refer this link **https://getcomposer.org/**  for "**How to install Composer**".

### Database Settings

	* Path - server/php/config.inc.php

    * define('R_DB_DRIVER', 'pgsql');
	* define('R_DB_HOST', 'localhost');
	* define('R_DB_NAME', 'DBNAME');
	* define('R_DB_USER', 'DBUSER');
	* define('R_DB_PASSWORD', 'DBPASSWORD');

### Create database for your project

* Import db from the script

 	sql/getlancer_with_sample_data.sql

# Front Side: 

### You need to install nodejs, bower, grunt.

Go to the path in command prompt. "/client/

* Run the below command, the bower used to download and installed all front-end development libraries.

        bower install

* The npm used to install the all dependencies in the local node_modules folder.

        npm install    

### Need write permission for following folders recursively
 
		/media
		/tmp
		/client/images
		/scripts(only main folder not recursive)				
		/server/php/Slim/shell
 
### Setting up cron
			
        ## Common
        	*/2 * * * * /##DOC_ROOT_PATH/##PROJECT_NAME/server/php/Slim/shell/main.sh 1» /##DOC_ROOT_PATH/##PROJECT_NAME/tmp/logs/shell.log 2» /##DOC_ROOT_PATH/##PROJECT_NAME/tmp/logs/shell.log

        ## Jobs Plugin
		    */2 * * * * /##DOC_ROOT_PATH/##PROJECT_NAME/server/php/Slim/shell/subscription.sh 1» /##DOC_ROOT_PATH/##PROJECT_NAME/tmp/logs/shell.log 2» /##DOC_ROOT_PATH/##PROJECT_NAME/tmp/logs/shell.log
		
		    */2 * * * * /##DOC_ROOT_PATH/##PROJECT_NAME/server/php/Slim/shell/job.sh 1» /var/www/html/tmp/logs/shell.log 2» /var/www/html/tmp/logs/job.log
     
