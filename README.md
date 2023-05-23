Install pymongo 

pip install pymongo


install Djongo

pip install djongo




DATABASES = {
    'default': {
        'ENGINE': 'djongo',
        'NAME': os.environ.get('DB_NAME'), #here
        'USER': os.environ.get('DB_USER'), #here
    #     'PASSWORD': os.environ.get('DB_PASS'), #here
    #     'HOST': '127.0.0.1',
    #     'PORT': '3306',
    #     'OPTIONS': {'init_command': "SET sql_mode='STRICT_TRANS_TABLES'"},
    }
}


//Migration Done

python manage.py makemigrations ||python manage.py migrate 



python3 manage.py collectstatic 

python manage.py runserver 127.0.0.1:8000
