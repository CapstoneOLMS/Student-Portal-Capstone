<p align="center"><img src="logo.jpg" height="140" alt="logo"/></p>
<h1 align="center">Student Portal 📚</h1>
<p align="center">Open Source Student Portal for Small Institutions!</p>
<p align="center">
<img alt="GitHub Pipenv locked Python version" src="https://img.shields.io/github/pipenv/locked/python-version/CapstoneOLMS/Student-Portal-Capstone">
<a href="https://img.shields.io/github/issues/CapstoneOLMS/Student-Portal-Capstone"><img alt="GitHub issues" src="https://img.shields.io/github/issues/CapstoneOLMS/Student-Portal-Capstone"></a>
<a href="https://img.shields.io/github/issues/CapstoneOLMS/Student-Portal-Capstone/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/CapstoneOLMS/Student-Portal-Capstone"></a>

![Website Image](./showcase.PNG)

## ⚡ Features

 **Multiple User Authentication** - Start with either a Teacher or a Student Account

 **Course Creation and Enrollment** - Teacher's Create Courses and Student Enroll and are able to access information

 **Notices/Results Creation** - Seperate Staff only access to CRUD Notices and Results

 **Quizzes** - Teacher's Create Multiple Choice Quizzes and Students can take them
  
 **Clean Tailwind UI** - Responsive design made from Tailwind CSS
  
 **Better Admin Interface** - Staff and Admin are utilized the old Django Jet Admin rebooted for Django 3 

> Many more features that you can explore yourself

## 🚀 How to Setup

These instructions will get you a copy of the project up and running on your local machine for deployement and development.

You'll need [Git](https://git-scm.com) and [Python 3.8+](https://www.python.org/downloads/) installed on your local computer.

```
python@3.8 or higher
git@2.17.1 or higher
```

You can also use the [Zip](https://github.com/CapstoneOLMS/Student-Portal-Capstone/archive/refs/heads/main.zip) file and extract the folder.

## 🔧 How To Use

From your command line, clone and deploy:

```bash
# Clone this repository
$ git clone https://github.com/CapstoneOLMS/Student-Portal-Capstone.git

# Go into the repository
$ cd portal-backend

# Install dependencies
# if Pipenv available ? run
$ pipenv install

# Else
$ pip install -r requirements.txt

```

## 📨 Environment Setup

```bash
# You'll need some environment variables
touch .env
# replace string with a random string
SECRET_KEY={string}
DEBUG=True
```

## 🛠️ Django Setup

After installing the requirements, we'll need to setup some Django commands.

### Perform database migration:

```bash
python manage.py check
python manage.py migrate
```

### Create Admin Account

> This is the admin account and only this user can login.

```bash
python manage.py createsuperuser
# follow instruction
```

### Create Staff Account

> You can create a group inside admin and make new staff users members in it. Not giving permissions by default is a security feature.

### Run Development Server

```bash
python manage.py runserver
```

Navigate to [http://localhost:8000/](http://localhost:8000/) endpoint in your browser.

Admin endpoint is at http://127.0.0.1:8000/admin/

## Important

The Readme is a work in progress, although the app is deployed.

## 📄 License

This project is licensed under the GPL3 License - see the [LICENSE.md](./LICENSE) file for details


#### Designed & Developed with love by ISU students(https://github.com/CapstoneOLMS)
