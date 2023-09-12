# MetarDecoder
This is a METAR code decoder project that decodes METAR weather reports based on the provided state code. It provides two API endpoints. This README.md file will guide you through setting up and running the project.

# Prerequisites
Before you start, make sure you have the following prerequisites installed on your macOS:

1: Python 3.9
3: virtualenv
4: pip (Python package manager)

# Installation
1. Create a folder and extract the source code
    cmd: tar -xzvf file_name.tar.gz
    example: tar -xzvf metar.tar.gz

2. open current directory in editor(VSCode)

3. Create a virtual environment to isolate project dependencies.
    virtualenv venv

4. Activate the virtual environment.
    source venv/bin/activate

5. Install project dependencies from the requirements.txt file.
    pip install -r requirements.txt

6. Make sure you are in the project directory and the virtual environment is activated.

7. move to the project directory containing file 'manage.py'
    say: cd /nws

8. start the server(at specific port 8080)
    python manage.py runserver or python manage.py runserver 8080

# API Endpoints
1. Ping
    URL: http://localhost:8000/metar/ping
    Method: GET
    Description: Check if the API server is running.
    Open browser and paste the URL.
    ex: http://localhost:8000/metar/ping

2. METAR Info
    URL: http://localhost:8000/metar/info
    Method: GET
    Query Parameters:
    scode (required): The state code for which you want to retrieve METAR information (e.g., CYLL).
    nocache (optional): Set to 1 to bypass caching and fetch the latest METAR data.
    ex: http://localhost:8000/metar/info?scode=CYLL&nocache=1

# In case the project setup didn't up and run proprly go to the link below
    url: 


# Contact
    Name: Sailesh Kumar
    Email: sailesh.18738@knit.ac.in
    GitHub: https://github.com/skumar5011987