# CloudServerjustifi
Documentation
===
    Documentation about sanctum Justfi codebase can be found here:
    http://sanctum.com/

Steps to setup Justifi
===
   Latest version: 1.0.0

1) Clone the adwyze assignment repo:

        git clone https://birendra7654@bitbucket.org/birendra7654/cloudserverjustifi.git

2) Create a virtual environment and install requirements

        # create virtual env in python 3
        virtualenv -p python3 envname
        source envname/bin/activate
        cd cloudserverjustifi
        pip install -r requirements.txt

4) Run the server

        python manage.py run
            OR
        gunicorn -w 4 -b 0.0.0.0:5000 manage:app

5) Follow this URl in Browser to see all API:

        http://127.0.0.1:5000/docs
