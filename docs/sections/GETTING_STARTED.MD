# GETTING STARTED WITH DJANGO 3.0
In this readme, we are going to break down step by step how our django application is configured, structured and set up.

## Creating a Virtual Environment
The virtualenv tool is a utility that separates projects and keep them in their own realm. We have some modules that can be shared by multitude of projects. These modules are usually installed once. But for some modules, it is recommended to isolate them for specific projects since they may vary in version from projects to projects.

What happens when you create a virtual environment is that some directories(`bin`, `include`, and `lib`) are created which hold a copy of the Python installation and some other shared resources. When this environment is activated, any thing installed with pip will be put in and used by the site packages of the virtual environment and not the global site packages of the python installation.

The virtual environment used here is [venv](https://docs.python.org/3/library/venv.html). The following steps were followed;
- Create the project directory: `$ mkdir django-prog`
- cd into that directory: `$ cd django-prog`
- run `$ python3 -m venv .venv --prompt django-prog`


**NB** `--prompt` provides an alternative prompt prefix for the environment.

- To activate the environment, we run the following in the project directory: `$ source .venv/bin/activate`. 

- To deactivate, we use `(django-prog)$ deactivate`

## Structuring the project file
A well structured project makes us well organized, productive and more focused on the business logic of our project. Here, I'll explain the file structure that is used by our django project.