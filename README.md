



<h1>Steps To Run</h1>

clone the project and type

    $ pip install -r requirements.txt
    
And to setup database do the following:
<ul>
<li>
first install sql if it is not present in your system
</li>
<li>
You can download it from https://www.mysql.com/downloads/
</li>
<li>
change your settings.py as following:-

DATABASES = {  
    'default': {  
        'ENGINE': 'django.db.backends.mysql',  
        'NAME': 'a8',  
        'USER': 'root',  
        'PASSWORD': '123',  
        'HOST': '127.0.0.1',  
        'PORT': '3306',  
        
}  
}
  


</li>
    <li>Password should be your mysql client password</li>
</ul>
then go to mysql client and do the following steps

    $ show databases;
    $ CREATE DATABASE a8;
  
    Then You Can Go Back To Your IDE Terminal And Do These Commands:-
    $ python manage.py makemigrations
    $ python manage.py migrate
    
    
And then:

    $ python manage.py runserver
