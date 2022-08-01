# **My-Shopping-Mart**

![Screenshot of website](https://user-images.githubusercontent.com/23288656/182156472-9d88340d-b471-4462-bb16-e2dc0301aacc.png)


This is a basic python-django based eCommerce shopping website

# **Prequisite to develope this project**

1 OS Linux-Ubuntu (Windows ,Mac)

2 Install IDE Visual Studio Code (you can use any code editor of your choice)
 download link--https://code.visualstudio.com/download

3 Install Python 
https://www.python.org/downloads/

4 Install Django 
https://www.djangoproject.com/download/

5 Backend tool - DB browser for SQLite
https://sqlitebrowser.org/dl/

6 Frontend tool- Bootstrap 
https://getbootstrap.com/docs/5.2/getting-started/introduction/

# **Steps to run this Shopping-Mart Website in your local host**

To get this repository, run the following command inside your git enabled terminal

Step 1
$ git clone https://github.com/prakashsanjay/My-Shopping-Mart.git

Step 2
$ python manage.py makemigrations

This will create all the migrations file (database migrations) required to run this App.

Step 3
Now, to apply this migrations run the following command

$ python manage.py migrate


Step 4

One last step and then our ecoomerce Shopping Mart website will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user

$ python manage.py createsuperuser

Step 5

 Now let's make the App live. We just need to start the server now and then we can start using our simple ecoomerce Shopping Mart. Start the server by following command

$ python manage.py runserver

Step 6 

Once the server is hosted, head over to http://127.0.0.1:8000/products/ for the App.That was pretty simple, right?

**feel free to update this project I will merge your updates into master branch**

Cheers and Happy Coding :)






