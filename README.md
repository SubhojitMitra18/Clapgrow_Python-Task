# 📝 Frappe To-Do List App

A simple To-Do List app built using the [Frappe Framework](https://frappeframework.com/).  
This app allows users to create, manage, and track their daily tasks efficiently.

## 🚀 Features
✅ Create and manage To-Do items
📅 Set due dates and priorities
🔁 Mark tasks as complete or pending
🧑 Assign tasks to specific users
📊 View filtered lists (Pending, Completed, Overdue)

## 🛠️ Installation

> Ensure you have [Frappe Bench](https://frappeframework.com/docs/v15/user/en/installation) installed.
Here is a **step-by-step command guide** to install and run your **Frappe To-Do List App** from scratch on a Unix-based system (e.g. Ubuntu with WSL):

## 🧰 Prerequisites

Make sure you have:

* Python 3.10 or 3.12
* Node.js (v16+), npm
* Redis
* Yarn
* wkhtmltopdf with Qt patches
* MariaDB or MySQL
* npm packages: `frappe-cli`

Refer to the official setup guide for your OS if needed:
👉 [https://frappeframework.com/docs/v15/user/en/installation](https://frappeframework.com/docs/v15/user/en/installation)

## 📦 Step-by-Step Installation of To-Do App

### 1. Set up Frappe Bench

# Install Frappe Bench CLI
pip install frappe-bench

# Initialize bench directory
bench init frappe-bench --frappe-branch version-15

# Go into the directory
cd frappe-bench


### 2. Create a Site

bench new-site todo.local
# Set MySQL root password and admin password when prompted

### 3. Get the To-Do App

If it’s your custom app:

bench get-app todo https://github.com/Noddy2003/Clapgrow_Task.git --branch main

Or if it’s the default Frappe ToDo app (used for learning):

bench get-app todo https://github.com/frappe/todo.git

### 4. Install the App on the Site

bench --site todo.local install-app todo

### 5. Start Development Server

bench start

Your site will now be running at:
🌐 [http://localhost:8000](http://localhost:8000)

## ✅ Summary of All Commands

pip install frappe-bench

bench init frappe-bench --frappe-branch version-15

cd frappe-bench

bench new-site todo.local

bench get-app todo https://github.com/Noddy2003/Clapgrow_Task.git --branch main

bench --site todo.local install-app todo

bench use todo.local

bench start
