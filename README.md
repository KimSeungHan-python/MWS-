# Django Blog

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

A simple blog application developed using the Django framework. This project was created for the **"Mobile Programming Web Service"** university course.

This project was fully completed and successfully deployed to **PythonAnywhere**, demonstrating all features in a live environment.

## ✨ Features

This application was built to support all the essential features of a blog:

* **Database Model:** A `Post` model defined in `blog/models.py` serves as the schema for all blog posts.
* **Full CRUD in Admin:** The Django Admin panel was configured to allow for full Create, Read, Update, and Delete (CRUD) operations on posts.
* **Dynamic Post List:** A main homepage view that queries the database and displays a list of all published posts.
* **Detailed Post View:** A separate view and template to display the full text of a single, specific post.
* **Korean Localization:** The project was configured in `settings.py` for Korean language and the Seoul timezone.

## 🛠️ Technical Stack & Concepts

This project is a practical application of Django's **MVT (Model-View-Template)** architecture.

* **Model (`blog/models.py`):**
    * Defines the `Post` schema with fields like `author`, `title`, `text`, `created_date`, and `published_date`.
* **View (`blog/views.py`):**
    * (In the full version) Contains the Python logic to fetch data from the database (e.g., `Post.objects.all()`) and pass it to a template.
* **Template (HTML Files):**
    * (In the full version) The user-facing HTML files that dynamically render the data provided by the Views.
* **Settings (`mysite/settings.py`):**
    * Manages all project-level configurations, including the `INSTALLED_APPS` (like `blog`), database connection (SQLite), and `ALLOWED_HOSTS` for deployment.
