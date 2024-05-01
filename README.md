Student Performance Portfolio

A modern Student Management System 👨‍🎓 with features like Interactive Dashboard 🤩 Attendance Management 🏫Provide Feedback ✍ Result Generation 📜 Leave Application 🍂A modern Student Management System 👨‍🎓 with features like Interactive Dashboard 🤩 Attendance Management 🏫Provide Feedback ✍ Result Generation 📜 Leave Application
🍂Development 👨‍💻

Note : Make sure you have Python version 3.8+

Environment Setup 🚀

$ git clone https://github.com/Akash1362000/Django_Student_Management_System.git

$ cd Django_Student_Management_System/

Create .env file (refer .env.example file)

Generate SECRET_KEY from here

Generate your CAPTCHA_SECRET from here

Copy your SITE KEY after generating CAPTCHA_SECRET and paste it in data-sitekey in student_management_app/templates/login_page.html (replace the current key with your key)

Database Setup



nstall Postgres Latest version from here

Install pgAdmin from here

Create a Database using pgAdmin by following the steps mentioned here

Update your DATABASE_URL in .env with your DB details like USER, PASSWORD and DB_NAME

If virtualenv is not installed (What is virtualenv?):

$ pip install virtualenv

Create a virtual environment

$ virtualenv venv

Activate the environment everytime you open the project

$ source venv/Scripts/activate

Install requirements 🛠

$ pip install -r requirements.txt

$ pre-commit install

Run migrations for Database

$ python manage.py migrate

Create superuser for Admin Login 🔐

$ python manage.py createsuperuser

Enter your desired username, email and password. Make sure you remember them as you'll need them in future.

eg.

Username: admin

Email: admin@admin.com

Password: HighlyConfidentialPassword
All Set! 🤩

Now you can run the server to see your application up & running 🚀

$ python manage.py runserver

To exit the environment ❎

$ deactivate

Every time you want to open the application in browser, make sure you run:

$ source venv/Scripts/activate

$ python manage.py runserver

Docker Setup (Optional) 
If you want to use Docker to run this project, you need to do the following steps:

Install Docker for your OS from here
Run docker --version and docker compose --version [In Windows, you need to run docker-compose --version to check the version]
If you see both the versions, then Docker is successfully installed on your system and you can follow along
If you don't see the version, check with your Docker installation
Open docker-compose.yml file and update the value of CAPTCHA_SECRET with your generated key. You can generate it from here
Run docker compose up -d
Run docker exec -it student_management_system sh -c "python manage.py createsuperuser" to create a new superuser
Access the app at http://localhost:8000
To stop the container, run docker compose stop from the project root
To restart the container, run docker compose start from the project root
To delete the container, run docker compose down from the project root
A Glimpse of the Dashboard 😍
Dashboard

Stargazers
Stargazers

Liked our work? 🤔 Do star this repository ⭐ It'll motivate us more 😁

License ✍
MIT License

Copyright (c) 2020 Akash Shrivastava

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
Releases
No releases published
Sponsor this project
patreon
patreon.com/shrivastava136
https://www.paypal.com/paypalme/akash1362
Packages
No packages published
Contributors
5
@Akash1362000
@dependabot[bot]
@akankshast
@ShreejitNair
@samiksha8888989
Languages
JavaScript
90.9%
 
CSS
6.0%
 
HTML
2.4%
 
Python
0.5%
 
Less
0.2%
 
Dockerfile
0.0%
Footer
© 2024 GitHub, Inc.
