# deploy

Setup
Update the System

   ***********************************                          sudo apt-get update      ++++++++++++++++++++++++++++++++++++++++++
To get this repository, run the following command inside your git enabled terminal

git clone https://github.com/yeshwanthlm/django-on-ec2.git
You will need django to be installed in you computer to run this app. Head over to https://www.djangoproject.com/download/ for the download guide

Download django usig pip

         +++++++++++++++++++++++++++++++++++++++++++++         sudo apt install python3-pip -y   ++++++++++++++++++++++++++++++++++
                +++++++++++++++++++++++++++++++++++++            pip install django         +++++++++++++++++++++++++++++++++++
Once you have downloaded django, go to the cloned repo directory and run the following command

 +++++++++++++++++++++++++++++++++++                        python3 manage.py makemigrations  ++++++++++++++++++++++++++++++++ 
This will create all the migrations file (database migrations) required to run this App.

Now, to apply this migrations run the following command

      +++++++++++++++++++++++++++++++++++++++++++++++++++       python3 manage.py migrate  ++++++++++++++++++++++++++++++++++++++++
One last step and then our todo App will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user

     ++++++++++++++++++++++++++++++++++++++++++++++++        python3 manage.py createsuperuser +++++++++++++++++++++++++++++++++++++
That was pretty simple, right? Now let's make the App live. We just need to start the server now and then we can start using our simple todo App. Start the server by following command

       +++++++++++++++++++++++++++++++++++                python3 manage.py runserver 0.0.0.0:8000       +++++++++++++++++++++++++++++++++++++++
Once the server is hosted, head over to http://127.0.0.1:8000/todos for the App.

Cheers and Happy Coding :)

                 
