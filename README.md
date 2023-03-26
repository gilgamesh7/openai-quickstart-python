# Copy of OpenAPI Quickstart from Open AI

## Links
[OpenAI Quickstart](https://platform.openai.com/docs/quickstart/build-your-application)

## Instructions for laptop
### Create repo from VSCode
1. shift+command+P
1. search for github
1. Publish to Github

### Poetry for venv
1. [Youtube - Poetry](https://www.youtube.com/watch?v=0f3moPe_bhk)
1. To Install
    1. pip install poetry
    1. pip3 install --upgrade pip
    1. poetry init
1. Recreate environment
    1. poetry config virtualenvs.in-project true
    1. poetry install
    1. Add/Remove
        1. poetry add (package name)
        1. poetry remove (package name)
1. List active venv : poetry env list

### Template for .env file
1. Create .env in .venv, to ensure you **do not inadvertantly upload your API KEY**
```
export FLASK_APP=app
export FLASK_ENV=development

# Once you add your API key below, make sure to not share it with anyone! The API key should remain private.
export OPENAI_API_KEY=
```

### Run on laptop
1. cd .venv
1. . ./.env
1. env (to check)
1. flask run

# OpenAI API Quickstart - Python example app

This is an example pet name generator app used in the OpenAI API [quickstart tutorial](https://beta.openai.com/docs/quickstart). It uses the [Flask](https://flask.palletsprojects.com/en/2.0.x/) web framework. Check out the tutorial or follow the instructions below to get set up.

## Setup

1. If you don’t have Python installed, [install it from here](https://www.python.org/downloads/).

2. Clone this repository.

3. Navigate into the project directory:

   ```bash
   $ cd openai-quickstart-python
   ```

4. Create a new virtual environment:

   ```bash
   $ python -m venv venv
   $ . venv/bin/activate
   ```

5. Install the requirements:

   ```bash
   $ pip install -r requirements.txt
   ```

6. Make a copy of the example environment variables file:

   ```bash
   $ cp .env.example .env
   ```

7. Add your [API key](https://beta.openai.com/account/api-keys) to the newly created `.env` file.

8. Run the app:

   ```bash
   $ flask run
   ```

You should now be able to access the app at [http://localhost:5000](http://localhost:5000)! For the full context behind this example app, check out the [tutorial](https://beta.openai.com/docs/quickstart).
