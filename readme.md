# Google cloud function course

## Starting new project with Python

To start new project in Google Cloud go to 
[firebase console]{<https://console.firebase.google.com}> or 
create from [Google Cloud Console platform]{<https://console.cloud.google.com}>

## Creating virtual environment

First we need to install 'python3-venv' with the following command.

```Bash
sudo apt install python3-venv
```

Then we execute the folowing command

```bash
python3 -m venv venv
```

Windows activation of env

```
venv\scripts\activate.bat
```

## Then we can add dependencies (packages) to 'requirements.txt' file and we can install them with:

```
pip install requirement.txt
```

## Deploying our functions

First set project ID with :

```
gcloud project list
gcloud config set project [project_id]]
```

Then we deploy our project with this command:

```
gcloud functions deploy [FUNCTION_NAME] --runtime python37 --trigger-http
```