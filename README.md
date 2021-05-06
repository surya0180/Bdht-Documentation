# Best Doctors & Hospitals Tracker
![](/images/image1.JPG)
* Best doctors and hospitals tracker is the name of the project we have built and the name of the website is ```JEEVAN NAKSHA```.
* In our website you can register in three ways :-
   1. You can register as an User if you are a normal user/patient.
   2. You can register as a Doctor if you are a Doctor.
   3. You can register as a Hospital if you are a Hospital.
* In recent days, online mode is very common in every industry and many people or customers are willing to use the online mode to complete their work.
* It's been a hard time for some users who are searching for some best doctors or hospitals nearby them, so that they can save their effort of searching via offline mode.
* Our Website ```JEEVAN NAKSHA``` will provide the users this facility to search for the doctors or hospitals near by them.
* User can even have an **appointment** with a particular doctor they like from our website.
* Every section of our website will be explained in the following [Documentation](#documentation).

# Documentation
* [Project-Installation](#Project-Installation)
* [Authentication](#Authentication)
* [Registeration](#Registeration)
* [Search-for-Doctors](#Search-for-Doctors)
* [Search-for-Hospitals](#Search-for-Hospitals)
* [How-to-view-Profiles](#How-to-view-Profiles)
* [How-to-update-Profiles](#How-to-update-Profiles)
* [How-to-add-reviews/ratings](#How-to-add-reviews/ratings)
* [Make-Appointment](#Make-Appointment)
* [Contributers](#Contributers)

## Project-Installation
### Project Environment
#### Following are the list of softwares required for the environment.
* Python 3 or more
* Django 3 or more
* pycopg package from python
* pillow package from python
* HTML5, CSS, Node.js Support
* Version control (Git, Github)
* Postgre sql server and PgAdmin
### Installation
#### Step-1 
Clone this repository **[link](https://github.com/WAD-Team-Alpha/Hospital_Review_System.git)** using this command in your terminal/command prompt.
```
git clone https://github.com/WAD-Team-Alpha/Hospital_Review_System.git
```
#### Step-2 
Navigate to public folder and create a python file with name **email.py**.\
![](/images/Capture.JPG)
#### Step-3 
Inside the **email.py** file create the list of variables mentioned below and assign them accordingly.
* ```EMAIL_HOST_USER```     This variable is used to store the **email** of the website
* ```EMAIL_HOST_PASSWORD``` This variable is used to store the **password** for the email of the website
* ```EMAIL_HOST```          This variable is used to mention the type of host **In our case we use smtp.gmail.com**
* ```DEFAULT_FROM_EMAIL```  This variable stores the **default email** used by the website
* ```DB_PASSWORD```         This is the password of the database used in the **settings.py** file in public folder
#### Step-4
Before you run the project, make sure that you apply all the migrations to your database. If you are using postgre sql use the following **command**
```
python manage.py sqlmigrate (App_name) (migration_number)
```
Here ```App_name``` is the name of the app which has the migration with migration number ``` migration_number ```
**Note:** that you should use the above command only if you are using the sql based database as your backend otherthan **sqlLite3** which is *default* one.
After you should migrate all the migrations using the following **command**.
```
python manage.py migrate
```
#### Step-5
After applying all the migrations, now its time to run the website. Make sure that you have your environment ready with all the mentioned softwares installed. In your command prompt/terminal run this command to start the **django server**.
```
python manage.py runserver
```

Hence the **installation** and setup of the project is **done completely**.

## Authentication
## Registeration
### A person can register in our website as follows
* If the person is a user or a patient, he can register using ```User Registeration``` form
* If the person is a doctor, he can register using ```Doctor Registertion``` form
* If the person has a hospital, he can register using ``` Hospital Registeration ```form
### Navigating to Signup page
* The page looks something **like this**


![](/images/cap2.JPG)
* Below is a small **Illustration** of how to navigate to signup page


![](/images/gif1.gif)

* You can register in any three of them depending on your ```profession```

## Search-for-Doctors
## Search-for-Hospitals
## How-to-view-Profiles
## How-to-update-Profiles
## How-to-add-reviews/ratings
## Make-Appointment
![](/images/cap3.JPG)
### Only a patient can have an appointment with a doctor
* Patient first needs to give the username of the doctor by viewing the ```username``` from the respective ```Doctor profile```
* Then he must mention the ```date of the appointment```
* And then mention the ```message``` required to convey his/her problem to the doctor
* Once the appointment is done, An email is sent to **both the respective doctor and the user** just for the confirmation.
* And then, the doctor will take up the converstaion with the user. This is the complete process of the appointment.
![](/images/gif2.gif)
## Contributers
