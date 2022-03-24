# Django Ecommerce

This is a simple Ecommerce application built with Django. This is a simple application developed with learning purposes in mind and contains just a few use cases of a real Ecommerce. So it might be incomplete or lack lots of features that real Ecomerce applications contains. The intention of this application is not to be a **REST** API, but a **MVT** (Model View Template) app.

## Set Up

In order to set up this project, you must have python (at least 3.8) installed in your computer with pip package manager. First, we must set up a virtual environment to isolate this project dependencies and avoid mess up with your local python environment. First, type on your console:

```
python -m venv venv
```

This command will create a folder called `venv` inside your project's folder and it will contain a copy of your local python environment, but isolated. Then, you should activate it.

Linux
```
source venv/bin/activate
```

Windows:
```
.\venv\Scripts\activate
```

With virtual environment created, now it's time to install dependencies. First, upgrade your package manager.

```
python -m pip install --upgrade pip
```

Now install your dependencies:

```
pip install -r requirements.txt
```

### Environment variables

This project comes up with a file named `.env.example` that contains some default configurations or environment variables names without value, if they have a sensitive value, like a secret key, api key or external service credentials.

### Infrastructure

This project comes with a `Dockerfile` and a `docker-compose.yml` to instantiate and orchestrate everything this project need to run.

On the first time, just type the following command to build the infrastructure locally:
```
docker-compose up --build
```

Otherwise:
```
docker-compose up
```