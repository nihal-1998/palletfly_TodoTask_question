# palletfly_TodoTask_question
To implement a Django REST API for a ToDo task, create a new Django app, define a Task model with relevant fields, create a TaskSerializer and TaskViewSet to handle CRUD operations, define URL patterns using DefaultRouter, and test using a tool such as curl or Postman.


ToDo Task API
This is a simple Django REST API for managing ToDo tasks.

Requirements
Python 3.x
Django 3.x
Django REST Framework 3.x
Installation
1) Clone the repository:
git clone https://github.com/nihal-1998/palletfly_TodoTask_question.git

2)Install the dependencies:
pip install -r requirements.txt


Usage
1) Start the development server:
python manage.py runserver

2) Access the API at http://localhost:8000/.


Endpoints
The following endpoints are available:

GET /tasks/: List all tasks
POST /tasks/: Create a new task
GET /tasks/<pk>/: Retrieve a specific task
DELETE /tasks/<pk>/: Delete a specific task
Examples
To list all tasks:

curl http://localhost:8000/tasks/


To create a new task:
curl -X POST http://localhost:8000/tasks/ -d '{"title": "Task 1", "description": "This is the first task."}' -H 'Content-Type: application/json'

To retrieve a specific task (replace <pk> with the ID of the task):
curl http://localhost:8000/tasks/<pk>/

To delete a specific task (replace <pk> with the ID of the task):
curl -X DELETE http://localhost:8000/tasks/<pk>/

