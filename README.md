# AWS EC2 Excercise

This cmd-line application has two features that displays ec2 instance/ingress rules information to the user.

# Running the Application

* The application can be launched using Windows Powershell/Command Prompt, or Bash (Linux). 
* Clone this repository into your local directory (requires git), or download the zip & extract

## Requirements

* [Python 3](https://www.python.org/downloads/) installed on your host machine
* pip (required for installing dependencies)
* git (optional, for cloning this repo)

Note: When cloning, use the HTTPS method. Python3, git and pip can installed with the respective package manager of your Linux distro (apt/yum), or by using the executable installers in windows (pip is included by default with Python version >3.4 in Windows).

## Setup Virtual Environment

* Using your terminal, cd to the application directory
* Create Virtual Environment:
```bash
python3 -m venv venv
```

* Activate Virtual Environment:
```bash
(Windows Command Prompt) venv\Scripts\activate
```
```bash
(Windows Powershell) venv/Scripts/activate (May need to run: Set-ExecutionPolicy RemoteSigned)
```
```bash
(Linux) source venv/bin/activate
```

* Install requirements into virtual env:
```bash
pip3 install -r requirements.txt
```

## Configure AWS credentials

* On the CLI, configure AWS settings by typing:
```bash
aws configure
```
* Paste in your AWS Access Key, Secret, and Region. Output format can be left as "None"

## Run the Application

```bash
python ec2_main.py
```

## Run Unit Tests
```bash
python -m unittest test_ec2.py
```

