# Dockerfile Bug: Missing Dependencies in Unittest
This repository demonstrates a common error in Dockerfiles: forgetting to install project dependencies before running tests.
The `bug.Dockerfile` attempts to run unit tests using `unittest discover` without installing necessary packages, leading to import errors.
The solution (`solution.Dockerfile`) addresses this by adding a step to install dependencies using `pip install -r requirements.txt`.  Ensure you have a `requirements.txt` file in the root directory listing your project's dependencies.
