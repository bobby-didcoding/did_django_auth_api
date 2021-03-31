# did_django_auth_api
Django project with a basic user authentication

Note: you will need API keys from Google, Facebook and Twitter

1) cd to development directory
2) mkvirtualenv did_django_auth_api
3) mkdir did_django_auth_api
4) clone repository to new directory
5) pip install -r requirements.txt
6) Update settings.py with your email API information

EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
EMAIL_HOST = 'XXX'
EMAIL_PORT = 'XXX'
EMAIL_USE_TLS = 'XXX'
EMAIL_HOST_USER = 'XXX'
DISPLAY_NAME = "Auth API demo email"
DONOT_REPLY_EMAIL_PASSWORD = 'XXX'


if DEBUG:

    TWILIO_ACC_SID = 'XXX'
    TWILIO_AUTH_TOKEN = 'XXX'
    TWILIO_NUMBER = 'XXX'

else:

    TWILIO_ACC_SID = 'XXX'
    TWILIO_AUTH_TOKEN = 'XXX'
    TWILIO_NUMBER = 'XXX'


7) python manage.py makemigrations
8) python manage.py migrate
9) python manage.py runserver
10) python manage.py createsuperuser
11) add your own details
12) visit http://localhost:8000/admin & sign in
13) Create 2 sites in /Sites/sites

localhost:8000
127.0.0.1:8000

14) Now create 3 social applications in Social Account/social applications
15) Create a new application
16) Select Google in the first drop down
17) Name it Google oauth
16) add the API key and Secret key in each object
17) Select the 2 sites & then save
18) Follow 15 through to 17 again for Facebook
19) Follow 15 through to 17 again for Twitter


20) https://localhost:8000 - Bob's your uncle!! 

