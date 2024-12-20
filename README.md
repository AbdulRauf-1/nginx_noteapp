# Simple Notes App
This is a simple notes app built with React and Django.

## Requirements
1. Python 
2. Node.js
3. React

## Installation
1. Clone the repository
```
git clone https://github.com/Hitstar53/notesapp.git
```
2. Create a virtual environment and activate it
```
virtualenv venv
source venv/bin/activate
```
3. Install the requirements
```
pip install -r requirements.txt
```
4. Run the server
```
python manage.py runserver
```

## Frontend - React
5. Open another terminal and navigate to the mynotes directory
```
cd mynotes
```
6. Install the dependencies
```
npm install
```
7. Run the app
```
npm start
```

## Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx` 

## Make a Dockerfile
Build the app
```
docker build -t notes-app .
```

Run the app
```
docker run -d -p 8000:8000 notes-app:latest
```

Run the command in terminal
```
curl -L http://127.0.0.1:8000
```

## Redirect Website 
The website is running locally. To redirect it.
```
nano /etc/nginx/sites-enabled/default
```

Add proxy_pass localhost link in location

Restart the nginx service
```
systemctl restart nginx
```

Now, to fetch our frontend. Go to mynotes/build, copy all files folder in build to /var/www/html




