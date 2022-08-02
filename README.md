# **Deploy My-Shopping-Mart Django App in AWS EC2**

![Screenshot of website](https://user-images.githubusercontent.com/23288656/182156472-9d88340d-b471-4462-bb16-e2dc0301aacc.png)


Please follow the Instructions to build & deploy this Django App in AWS EC2 

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


 # *How To Deploy Django Application in AWS EC2*

Django comes with a development server that helps run Django projects in localhost. However, to make your web application available worldwide you will need a host machine. Amazon Web Services (AWS) provides EC2 (Elastic Compute Cloud) which is the most popular choice to host Django web applications.

# *Creating EC2 Instance With Ubuntu*

Step 1: Select EC2 From AWS Console and click lauch Instance

![Capture-ec2-2](https://user-images.githubusercontent.com/23288656/182432809-b2c4a14f-a482-4cc9-97b9-8cfd0e014f89.PNG)

Step 2: Name your Instance and Select Ubuntu 

![Capture-ec2-3](https://user-images.githubusercontent.com/23288656/182433167-3611baa9-7236-4854-9440-f29134f62408.PNG)


Step 3: 
select instance type t2-micro (make sure free tier eligible) and create new key pair

![Capture-ec2-4](https://user-images.githubusercontent.com/23288656/182433574-8191cd03-e577-4c13-ac09-75e749b2744c.PNG)


Step 4:

Select launch Instance

![Capture-ec2-6](https://user-images.githubusercontent.com/23288656/182440307-66b4b40d-a53d-46a3-bfc9-c9cfb179bd75.PNG)


Step 5:

If Instance created Succesfully you can view instance

![Capture-ec2-7](https://user-images.githubusercontent.com/23288656/182440371-c9e02e5b-a3da-42c8-ae1f-aae8f8a4a189.PNG)


Step 6:

Check instance is running and check status 2/2 passed

![Capture-ec2-8](https://user-images.githubusercontent.com/23288656/182440406-d67af11a-9951-4dd9-aae5-7860c8e67869.PNG)

Step 7

Now select security and edit inbound rule

![Capture-ec2-9](https://user-images.githubusercontent.com/23288656/182440992-29a1a169-7dc1-45ba-a99c-8043f08078ac.PNG)
![Capture-ec2-10](https://user-images.githubusercontent.com/23288656/182441324-68cd4780-4356-43e7-b7d2-598b2ed90e09.PNG)

Step 8:

In this Security setting add rules and edit inbound rule select custop TCP--Port range 8000 and source 
port 0.0.0.0 it will allow excess to anywhere click save rules

![Capture-new](https://user-images.githubusercontent.com/23288656/182441867-7c75cee1-d55b-4d72-b854-905716d1db83.PNG)

Step 9:

Now go back to your EC2 page select your instance and right click connect

![Capture-13](https://user-images.githubusercontent.com/23288656/182442973-35df0f2f-ac7f-40bd-8135-733083559df1.PNG)












**feel free to update this project I will merge your updates into master branch**



Cheers and Happy Coding :)






