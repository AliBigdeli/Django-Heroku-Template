<h1 align="center">Django Heorku Template Project</h1>
<h3 align="center">A simple start for any heroku project</h3>
<p align="center">
<a href="https://www.python.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a>
<a href="https://www.djangoproject.com/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/django/django-original.svg" alt="django" width="40" height="40"/> </a>
<a href="https://www.django-rest-framework.org/" target="_blank"> <img src="https://www.django-rest-framework.org/img/logo.png" alt="sqlite" width="90" height="40"/> </a>
<a href="https://getbootstrap.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a>
<a href="https://www.w3.org/html/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">
</a>
<a href="https://www.sqlite.org/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/sqlite/sqlite-icon.svg" alt="sqlite" width="40" height="40"/> </a>
<img src="https://www.vectorlogo.zone/logos/heroku/heroku-icon.svg" alt="heroku" width="40" height="40"/>
</p>


### Overview
- [Overview](#overview)
- [Goal](#goal)
- [Setup](#setup)
- [Getting ready](#getting-ready)
- [Repo Features](#repo-features)
- [Configurations](#configurations)
- [Deploy with HerokuCLI](#deploy-with-herokucli)
- [Deploy with Github](#deploy-with-github)
- [Deploy with OneClick](#deploy-with-oneclick)



### Goal
This project main goal is to provide a way to deploy django applications by using heroku ,gunicorn or even using one click deployment.


### Setup
To get this repository, run the following command inside your git enabled terminal
```bash
git clone https://github.com/alibigdeli/Django-CBV-DRF-ApiView-TodoApp
```

### Getting ready
Create an enviroment in order to keep the repo dependencies seperated from your local machine.
```bash
python -m venv venv
```

Make sure to install the dependencies of the project through the requirements.txt file.
```bash
pip install -r requirements.txt
```

Once you have installed django and other packages, go to the cloned repo directory and run the following command

```bash
python manage.py makemigrations
```

This will create all the migrations file (database migrations) required to run this App.

Now, to apply this migrations run the following command
```bash
python manage.py migrate
```

### options
Project it self has the user creation form but still in order to use the admin you need to create a super user.you can use the createsuperuser option to make a super user.
```bash
python manage.py createsuperuser
```

And lastly let's make the App run. We just need to start the server now and then we can start using our simple todo App. Start the server by following command

```bash
python manage.py runserver
```

Once the server is up and running, head over to http://127.0.0.1:8000 for the App.

### Reformat and check
If you want your code to be check by pep8 and all the guide lines, there are two packages added to requirements in order to check and reformat code.
you can use it by this command:
```bash
black -l 79 . && flake8
```

### Repo Features
<ul>
  <li>
       <strong>Latest LTS Django3.2</strong>        
  </li>
 <p>Latest LTS included 3.2.x and needed requirements</p>
 <li>
       <strong>Git</strong>        
  </li>
  <p>python gitignore and README with license</p>
 
 <li>
       <strong>Django env</strong>        
  </li>
  <p>enviroment sample file and setup</p>
 
 <li><strong>Base Restframework Authentication and Token</strong></li>
  <p>A simple login and registration page for starting project and testing</p>
 
 <li><strong>Black</strong></li>
  <p>Reformating your codes to standard projects</p>
 

 <li><strong>Travis and Flake8</strong></li>
  <p>Included with travis.yml configuration file for test purposes.plus included Flake8 and config files.</p>
 <li>
       <strong>Preconfigured</strong>        
  </li>
  <p>Preconfigured settings.py for db,static,media etc.</p>
</ul>


### Configurations

<ul>
  <li>
       <strong>Static & Media Directories</strong>        
  </li>
 <p>STATIC_ROOT and STATIC_URL and same for media configurations with STATICFILES_DIRS</p>
 <li>
       <strong>Template Directories</strong>        
  </li>
  <p>Genral templates directory for root</p>
 <li>
       <strong>Site Framework and Sitemaps + robots</strong>        
  </li>
  <p>Siteframework as in site_id configs with robots.txt and sample sitemaps</p>
  
 <li>
       <strong>Database Configs</strong>        
  </li>
  <p>Database configuration for production with postgresql and volume directory in data</p>
  
 <li>
       <strong>Email Configs</strong>        
  </li>
  <p>Email configurations for dev and prod as in env file</p>
 
 <li>
       <strong>Message Configs</strong>        
  </li>
  <p>Message and warnings configuration for notification handelings</p>
 <li><strong>Hints and Files</strong></li>
  <p>Sample files and hints all over the template for giving more pace</p>
  <li>
       <strong>Security</strong>        
  </li>
  <p>Security tags for https and redirections,HSTS,Cookie and other headers</p>
</ul>

### Deploy with HerokuCLI
https://devcenter.heroku.com/articles/git

### Deploy with Github
https://devcenter.heroku.com/articles/git

### Deploy with OneClick
https://devcenter.heroku.com/articles/heroku-button
