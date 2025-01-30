## Project Overview

A basic notes API that provides CRUD operations for managing notes. Built with Django and django-tastypie, this project serves as a learning exercise for understanding API development with Django.

## Features

- RESTful API endpoints for notes
- CRUD operations:
  - GET /api/note/ (list all notes)
  - GET /api/note/1/ (get specific note)
  - POST /api/note/ (create note)
  - PUT /api/note/1/ (update note)
  - DELETE /api/note/1/ (delete note)
- Automatic timestamp tracking for notes

## Tech Stack

- Python 3.13
- Django 5.1.5
- django-tastypie
- SQLite

## Setup

1. Clone the repository:
- bash
- git clone https://github.com/yourusername/notable_django.git
- cd notable_django


2. Create and activate virtual environment:
- bash
- python -m venv venv
- source venv/bin/activate # On Windows: venv\Scripts\activate

3. Install dependencies:
- bash
- pip install 
- pip install -r requirements.txt

4. Run migrations:
- bash
- python manage.py makemigrations
- python manage.py migrate

5. Run the server:
- bash
- python manage.py runserver

6. Access the API:
- Open your browser or use a tool like Postman and navigate to http://127.0.0.1:8000/api/note/ to see the notes.

## Project Structure
notable_django/
├── api/
│ ├── models.py # Note model definition
│ └── resources.py # API resource configuration
├── notable_django/
│ ├── settings.py # Project settings
│ └── urls.py # URL configuration
└── manage.py # Django management script


## Learning Outcomes

This project helped me understand:
- Django project structure
- RESTful API concepts
- Working with django-tastypie
- Basic database operations
- API endpoint configuration

## Note

This is a learning project and not intended for production use. The current setup uses basic authorization suitable only for development.

## License

MIT License
