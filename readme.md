# Django Rest Scaffolding



## Requirements

#####Recommended editor:
- **Open Source:**  [Visual Studio Code](https://code.visualstudio.com/Download), [PyCharm Community Edition](https://www.jetbrains.com/pycharm/download/), [ATOM](https://atom.io)

- **Proprietary:** - [PyCharm](https://www.jetbrains.com/pycharm/download/), [Sublime](https://www.sublimetext.com/3)



#####Prerequisite knowledge:

[Python](https://www.python.org), [Django](https://www.djangoproject.com), [MySQL](https://www.mysql.com), [Virtual Environment](https://docs.python.org/3/library/venv.html)



#####System requirements:

- Python Version : 3.6 or later
- Django Version : 2.0 or later
- MySQL Version : 8.0 or later



### Getting Started

1. *[Create a virtual environemnt](https://gist.github.com/IamAdiSri/a379c36b70044725a85a1216e7ee9a46) (Recommend to use [Virtual Environment Wrapper](https://virtualenvwrapper.readthedocs.io/en/latest/))*
```sh
mkvirtualenv --python=`which python3` scaffolding -r requirements.pip
```

**Note:** if you face error related to the `mysqlclient`  (Optional)

```sh
sudo pip install mysqlclient
```



2. *Create a project database using MySQL console*
```sh
mysql -u root -p
```
```sh
create database scaffolding-development;
```



3. *Set environment*
```sh
cp .env.sample .env
```
**Note:** update `.env` file variables as per your requirements.



#### Commands

- `python manage.py runserver` - For starting development server.
- `python manage.py runserver --settings=main.settings.production` - For starting production server.
- `python manage.py shell` - For starting intractive python shell.
- `python manage.py makemigrations articles` - For creating app migrations.
- `python manage.py migrate` - For applying migrations.
- `pip freeze` - To view installed python packages.



#### Dependencies

- [Django](https://pypi.org/project/Django/)

- [mysqlclient](https://pypi.org/project/mysqlclient/)

- [python-decouple](https://pypi.org/project/python-decouple/)

- [djangorestframework](https://www.django-rest-framework.org)

- [ipython](https://pypi.org/project/ipython/)

  


#### Future Enhancement

- Add comments to all the files
- Add unit test cases



#### Contributing

1. Fork it ( https://github.com/TuxEducation/django_rest_scaffolding/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new pull request.