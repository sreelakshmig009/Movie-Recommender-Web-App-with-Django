### Preview of how the app looks like

![SS1](/dmr(1).png )

![SS2](/dmr(2).png)

### Steps to run the Web App in your local ystem

After forking the main repository move to Django projects folder and follow the below the steps.

#### Create and start a a virtual environment

```
virtualenv env --no-site-packages
source env/bin/activate
```

#### Move to Movie-Recommender-With-Django

```
cd Movie-Recommender-With-Django
```

#### Install the Dependencies

```
pip install -r requirements.txt
```

#### Create superuser to access the admin page

```
python manage.py createsuperuser
```
Enter the Username of your choice and press enter.

```
Username: (your preferred username)
```
Enter the Email address and press enter.(It can be left blank)

```
Email address: something@gmail.com
```
Next, enter the Password in-front of the Password field and press enter.Enter a strong password so as to keep it secure

```
Password: ******  
```
Then again enter the same password for confirmation.

```
Password(again): ******
```
Superuser will be created successfully

#### Make database migrations

Django has sqlite database by default. If you want you can any sql or nosql database too. In this project I have used sqlite db.

```
python manage.py makemigrations movierecommender
```
Then run 
```
python manage.py migrate
```
#### Start the development server

To run the web app,run
```
python manage.py runserver
```
And open localhost:8000 and navigate to /movierecommender to see the running app or /admin to open the django administration

```
127.0.0.1:8000/movierecommender 
```
or 
```
127.0.0.1:8000/admin
```
