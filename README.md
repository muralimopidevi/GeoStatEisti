![PyPI - Python Version](https://img.shields.io/badge/Python-3.7-brightgreen)
![PyPI - Python Version](https://img.shields.io/badge/Django-3.1-green)
![PyPI - Python Version](https://img.shields.io/badge/requirements.txt-updated-yellow)
# GeoStatEISTI
## Purpose of Plan
The Geographical statistics of engineering internships Plan will provide a definition of the project, including the 
project’s goals and objectives. Additionally, the Plan will serve as an agreement between the following parties: Project
Sponsor, Steering Committee, Project Team, and other personnel associated with and/or affected by the project.

## Preview
![Project Preview](https://github.com/mopidevimu/GeoStatEisti/blob/master/ReadMe_pics/project.gif)

## Usage

```python
STEP-1

# Move to "GeoStatEisti" Folder and install required packages.
# by using "requirements.txt" file and open command prompt or terminal.
# run the following command.

    pip install -r requirements.txt

STEP-2
 
# After successful installation of packages run the following commands.
# on  command prompt or terminal.

# To Make Migrations.
    python manage.py makemigrations

# Migrate models to database.
    python manage.py migrate

# Create Super User (ADMIN).
    python manage.py createsuperuser

# The above command ask for username, email, password.
# provide those details to login to the website.

# To runserver or run project.
    python manage.py runserver

STEP-3

# Then open the following url Login with your username and password.
    http://127.0.0.1:8000/admin/

# Then goto DASH section click on 
# "Colleges" then import the CSV file which is provided in CSV FOLDER "stud_college.csv"
# "Countrys",then import the CSV file which is provided in CSV FOLDER "Country.csv"
# "Students",then import the CSV file which is provided in CSV FOLDER "stud_file.csv"
# "Internships",then import the CSV file which is provided in CSV FOLDER "stud_internship.csv"
# After uplaoding all CSV files logout from ADMIN PANEL.

STEP-4
# Use this url to login as USER.
    http://127.0.0.1:8000/

STEP-5

# For forget password we need to add email and password at
# MovieRating/MovieRating/settings.py file
# end of the settings you need to change these 2 lines like this

    EMAIL_HOST_USER = 'youremailid@gmgg.com'
    EMAIL_HOST_PASSWORD = 'yourpassword'

# Instead of these below lines

    EMAIL_HOST_USER = os.environ.get('EMAIL_USER')
    EMAIL_HOST_PASSWORD = os.environ.get('EMAIL_PASS')

# If you want to use above format Add the following Environmental Varibales in your windows.
    EMAIL_USER -> <user@gg.com>
    EMAIL_PASS -> <your email pass>


```

Hint:   change your database connetion to sqlite3 to any other
        "DATABASE" like MYSQL to perform opeartion past.