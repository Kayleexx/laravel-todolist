# Laravel TodoList App

A simple Todo List application built with **Laravel** that demonstrates creating, retrieving, updating, and deleting (CRUD) records from a database.

## Features

* Create new tasks with descriptions
* View all tasks in a clean list format
* Mark tasks as **completed**
* Delete completed tasks
* Styled with Bootstrap for a simple UI

## Requirements

* PHP >= 8.0
* Composer
* Laravel >= 10
* A database (MySQL, SQLite, or PostgreSQL)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Kayleexx/laravel-todolist.git
   cd todolist-app
   ```

2. Install dependencies:

   ```bash
   composer install
   ```

3. Copy the example environment file and configure your database:

   ```bash
   cp .env.example .env
   ```

   Update the `.env` file with your database details:

   ```
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=todolist
   DB_USERNAME=root
   DB_PASSWORD=
   ```

4. Generate an application key:

   ```bash
   php artisan key:generate
   ```

5. Run migrations to create the tasks table:

   ```bash
   php artisan migrate
   ```

6. Start the development server:

   ```bash
   php artisan serve
   ```

7. Open the app in your browser:

   ```
   http://127.0.0.1:8000
   ```

## Usage

* Visit the home page to see your task list.
* Click **New Task** to add a task.
* Click **Complete** to mark a task as completed.
* Click **Delete** to remove a completed task.

## Project Structure

* **Controller:** `app/Http/Controllers/TasksController.php`
* **Model:** `app/Models/Task.php`
* **Views:** `resources/views/tasks/`
* **Routes:** `routes/web.php`

