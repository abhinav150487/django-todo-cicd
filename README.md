# django-todo
A simple todo app built with Django.

## Application Screenshot

![Todo App](https://raw.githubusercontent.com/shreys7/django-todo/develop/staticfiles/todoApp.png)

## Jenkins CI/CD Pipeline

This project uses a Jenkins Declarative Pipeline to automate the CI/CD workflow. The pipeline performs the following stages:

- Checkout
- Build Docker Image
- Run Django Tests
- Deploy Docker Container

### Pipeline Screenshot

![Jenkins Pipeline](pipeline.png)

### Setup

To get this repository, run the following command inside your git enabled terminal

```bash
git clone https://github.com/abhinav150487/django-todo-cicd.git
```
