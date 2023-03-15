## Hi There :smiley:

# This is a hard coded version of how you would create a python & django website with a step by step guide below.

## TIPS :dizzy_face:
<!-- 1 -->
# What is virtualenv/virtual enviroment?
# virtualenv is used to manage Python packages for different projects. Using virtualenv allows you to avoid installing Python packages globally which could break system tools or other projects. You can install virtualenv using pip.

## INSTALLATION STEPS :shushing_face:
<!-- (support link https://linuxhint.com/activate-virtualenv-windows/) -->
<!-- INSTALLATIONS -->
# 1. install python
# 2. make sure you have " pip " installed
# 3. install virtualenv by runing " pip3 install virtualenv " in CMD
# 4. run " pip3 freeze " in CMD to check if virtual env was installed

<!-- CD to folder of your choice -->
# 5. run " cd [add folder name] " in CMD

<!-- Create virtual enviroment/virtualenv -->
# 6. run " virtualenv [Django_BlogCourse/File name of choice] " in CMD

<!-- activate virtualenv -->
# 7. run " Django_BlogCourse\Scripts\activate " in CMD/TERMINAL

<!-- cd to folder -->
# 8. run " cd [Django_BlogCourse/add folder name] " in CMD

<!-- Install Django -->
<!-- https://linuxhint.com/activate-virtualenv-windows/ -->
<!-- Check that the version your installing has LTS, Long.Term.Support for a more stable experience -->
# 9. run " pip install Django==2.2.2 "
<!-- if it already exists you can uninstall it by running " pip uninstall django " and install a new version -->

<!-- This will install a folder called mysite that you will need...after it is you can change the name to whatever: standard name is " src " -->
# 10. run " django-admin startproject mysite "

<!-- cd to the mysite folder/src folder if you changed the name -->
# 11. run " cd src/mysite "

<!-- run manage.py found in the src folder to run the server -->
# 12. run " python manage.py runserver " 
<!--  http://127.0.0.1:8000/ <-This is the default link you will be given if it was ran successfully -->
<!-- Once ran you will see a file called " db.sqlite3 " in the src folder-->

<!-- create a txt file to view all modules/packages/ect.. that is installed in this virtualenv -->
# 13. run " pip3 freeze > requirements.txt "
<!-- run this code everytime you pip install something -->

<!-- only use this to  install everything in the requirements.txt file when you clone this project/deploy the project -->
# 14. run " pip3 install -r requirements.txt "

## CREATE WEBSITE STEPS :shushing_face:

<!-- start app(make sure you are in the src folder) -->
# 1. run " python manage.py startapp personal "
<!-- after runing this you'll see a personal folder found in the src folder -->
<!-- everytime you add an app you have to add it to the mysite folder/settings.py file inside of the installed apps function -->

# 2. Create a folder called templates in src which is where you html files will be stored
<!-- after this go to setting.py and under the templates funtion add " os.path.join(BASE_DIR, 'templates') " into the DIR:[] -->

# 3. add html file found in templates to views.py found in the personal folder app

# 4. then you would go to mysite folder found in the src folder and open urls.py to link the html file to the app

# 5. inside the personal folder create a folder called templates and then inside templates create another folder called personal which is the app name

# 6. create a home.html file and add content blocks in both html files

# 7. repeate the linking steps for the new html file