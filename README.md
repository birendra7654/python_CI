# CI example of python with JENKINS
Documentation
===
    Documentation about ***
    https://realpython.com/python-continuous-integration/?fbclid=IwAR1jJLLN3tpMgfRw6RgocEdvPpBGpQAx8cpXIdNFsevrXZ8ERzuzQ7fHN6A

Steps to setup python with JENKINS
===
   Latest version: 1.0.0

1) Clone the python JENKINS  assignment repo:

        https://github.com/birendra7654/python_CI.git

2) Create a virtual environment and install requirements

        # create virtual env in python 3
        virtualenv -p python3 envname
        source envname/bin/activate
        cd python_CI
        pip install -r requirements.txt

4) Simple Calculator library and should zen of python rule

	flake8 --statistics

5) Run unit test cases.

	pytest -v --cov
