# gitlab-search
Python's script to search texts in any project

### Requirements
The script has been executed successfully with Python 3.8.5

### Installation
In order to do work the script you can create a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Alternatively, if you are working on Ubuntu or similar you can install required package:

```bash
sudo apt install python3-gitlab
```

### Usage

```
usage: gitlab-search.py [-h] GITLAB_SERVER GITLAB_USER_TOKEN FILE_FILTER TEXT_TO_SEARCH [GROUP] [PROJECT_FILTER]

positional arguments:
  GITLAB_SERVER      URL of Gitlab server, eg. https://gitlab.com/
  GITLAB_USER_TOKEN  Access token with api_read access
  FILE_FILTER        Filter for filenames to search in
  TEXT_TO_SEARCH     Text to find in files
  GROUP              Group to search for projects in, can be subgroup eg. parent_group/subgroup/another_subgroup
  PROJECT_FILTER     Filter for project names to look into

optional arguments:
  -h, --help         show this help message and exit
```
