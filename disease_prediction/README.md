### General Disease Prediction based on symptoms provided by patient- powered by Django & Machine Learning


# How To Use This
First makesure to install django and python in your local system
Then install the postgreSQL database with pgadmin4 in your system by using the link- https://www.postgresql.org/download/windows/
Then you have to manually create a DB instance on PostgreSQL by right clicking on the databases icon named "predico"....

Now go to the settings.py file.Under the settings for Databases, change the settings from sqlite3 or your current database to the following:
  DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'predico',   #your database name
        'USER': 'postgres',  #username of your database
        'PASSWORD': 'root',  #password of the database which u setup while the installation 
        'HOST': 'localhost', 
        'PORT':'',
    }
}

Then open the cmd go to your project folder then execute these commands:
   - pip install psycopg2
   - pip install pillow
  or you can execute these commands at system level also rather than at project level,anything is good enough

 Now go to your project folder
   - Make a new environment with the command-> py -m venv env
   - Run env\Scripts\activate command to activate the environment
   - Run pip install django
   - Go to main project folder(in my case it is disease_prediction)
   - Run pip install -r requirements.txt to install dependencies
   - Run python manage.py makemigrations
   - Run python manage.py migrate
   - Run python manage.py runserver
   - Navigate to http://127.0.0.1:8000/ in your browser

To create admin for your project,
   - Run python manage.py createsuperuser then
        it asks for username,email and password..enter them then superuser will be created successfully

### Dataset used - 
https://www.kaggle.com/neelima98/disease-prediction-using-machine-learning

### Some Sceenshots of This Webapp -

![](https://github.com/anuj-glitch/Disease-Prediction-using-Django-and-machine-learning/blob/master/screenshots/Capture1.PNG)
![](https://github.com/anuj-glitch/Disease-Prediction-using-Django-and-machine-learning/blob/master/screenshots/Capture2.PNG)
![](https://github.com/anuj-glitch/Disease-Prediction-using-Django-and-machine-learning/blob/master/screenshots/Capture3.PNG)
![](https://github.com/anuj-glitch/Disease-Prediction-using-Django-and-machine-learning/blob/master/screenshots/Capture4.PNG)
![](https://github.com/anuj-glitch/Disease-Prediction-using-Django-and-machine-learning/blob/master/screenshots/Capture5.PNG)


### ***Go to the [Readme.pdf](Readme.pdf) file for detailed information about the project & screenshots.***
and if you like this project, do give it a "Star" Thank you..
