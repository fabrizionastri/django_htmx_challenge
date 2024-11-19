# Django HTMX Calculator

<!-- Note is the a draft README file, to be updated/modified by the candiate -->

### Description

This applicable is a simple Django app that allows the user to store the products in a database, and to display them in a list. The user should be able to click on a product in the list to see the details of the product, and to edit the product.
The user can provide the price and tax information for the product in a flexible way, and the app will calculate the missing value.

### Installation

- `python -m venv .venv`: to create a virtual environment in the root folder
- `.venv\Scripts\activate`: to activate it using a build in script
- `pip install -r requirements.txt`: install all the dependencies with
- `python manage.py makemigrations`: make the migrations
- `python manage.py migrate`: run the migrations
- `python manage.py runserver`: start the server

### Usage

- Open browser on http://localhost:8000/ to see the app
