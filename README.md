# README #

Django vs angular 2 webpack: Blog sample


- Request django, nodejs npm, postgre
	+ Install django 1.10: 
	
		sudo apt-get update
		
		sudo apt-get install python3-pip
		
		sudo pip3 install virtualenv
		
		sudo pip3 install django==1.10
		
		
	+ Install nodejs npm:
	
		sudo apt-get update
		
		curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
		
		sudo apt-get install -y nodejs
		
	+ Install postgre:
	
		sudo apt-get update
		
		sudo apt-get install postgresql postgresql-contrib
		
		
		+ Create database: 
		
			sudo -u postgres psql
			
			CREATE DATABASE blog_angular2;
			
			
		+ Change password user postgres:
		
			sudo -u postgres psql
			
			ALTER USER postgres PASSWORD '12345';
	
- Run project:

	+ Start django:
	
		virtualenv --python=python3 env
		
		source env/bin/activate
		
		cd blogs/source
		
		pip3 install -r requirements.txt
		
		python3 manager makemigrations
		
		python3 manager migrate
		
		python3 manager runserver
		
	+ Build angular 2 new tab:
	
		cd blogs/source/source
		
		npm install
		
		npm run build-watch
		
		
* Update websocket:

	+ Start websocket:
	
		python3 server.py
