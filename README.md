# Task Manager To-Do List - Backend

This is the backend for a Task Manager To-Do List application built using Laravel. This backend API allows you to manage tasks with CRUD operations.
You will also need frontend part for this project, you can find it in my another repository.

## Table of Contents
- [Installation](#installation)
- [Environment Setup](#environment-setup)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Database Migration](#database-migration)
- [Contributing](#contributing)
- [License](#license)

## Installation

To get started with the project, clone the repository and install the dependencies:

```bash
git clone https://github.com/YourUserName/Task-Manager-To-Do-List-Backend.git
cd Task-Manager-To-Do-List-Backend
composer install
cp .env.example .env
php artisan key:generate
```

## Environment Setup

You need to create your own `.env` file based on the `.env.example` provided. This file contains all the environment variables required to run the application. I cannot put sensitive information like database passwords or API keys in public repositories.

## Usage 
Run the following command to start the development server:
```bash
php artisan serve
```
The application will be available at `http://localhost:8000`.

## API Endpoints

The following API endpoints are available:

`GET /api/tasks` - Retrieve all tasks
`POST /api/tasks` - Create a new task
`GET /api/tasks/{id}` - Retrieve a specific task by ID
`PUT /api/tasks/{id}` - Update a specific task by ID
`DELETE /api/tasks/{id}` - Delete a specific task by ID

## Database Migration

To set up the database, run the following command to apply the migrations:

```bash
php artisan migrate
```
Migration File: xxx_create_tasks_table.php

***Controllers:***

**TaskController.php**
This controller handles all the CRUD operations for the tasks.

***Models:***

**Task.php**
The model representing the tasks in the database.

***Providers:***

**AppServiceProvider.php**
This provider sets up the API routes.

***Routes:***

**api.php**
Defines the API routes for the application.

## Contributing
Contributions are welcome! Please fork this repository and create a pull request to submit your changes.

## License
This project is not currently licensed. If you wish to use the code for commercial purposes, please contact me to discuss licensing options.
