ZendDemoApplication
=======================

Introduction
------------
This is a simple, demo application using the ZF2 MVC layer and module
systems. I have added Ablum part.

Preview
-------
![perview](preview.jpg)
Dierectory
----------
	-| www
		-| ZendFramework-2.3.1/library
		-| zf20

Data
----
You should create a database named demo, and then run the album.sql.
 
Virtual Host
------------
Afterwards, set up a virtual host to point to the public/ directory of the
project and you should be ready to go!


	-| www
		-| vhosts
			-| httpd-vhost.conf

the conent in httpd-vhost.conf:

	<VirtualHost *:80>
	ServerName b.com
	DocumentRoot "D:\wamp\www\zf20\public"
	SetEnv APPLICATION_ENV "development"
	<Directory "D:\wamp\www\zf20\public">
	    DirectoryIndex index.php
	    AllowOverride All
	    Order allow,deny
	    Allow from all
	</Directory>
	</VirtualHost>
	
	
	<VirtualHost *:80>
	ServerName localhost
	DocumentRoot "D:\wamp\www"
	SetEnv APPLICATION_ENV "development"
	<Directory "D:\wamp\www">
	    DirectoryIndex index.php
	    AllowOverride All
	    Order allow,deny
	    Allow from all
	</Directory>
	</VirtualHost>
	
