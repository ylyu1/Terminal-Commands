1. cd to the folder where you want to store this virtural environment for this specific project e.g.
   pc:  ```c:/dev/jobfindchatbot``` 
   mac: ```~/dev/jobfindchatbot``` 
2. create virtual environment

``` sh
python -m venv venv
```
to specify the python version being used for the virtual environment, for example, to use python 3.12
```sh
python3.12 -m venv <virtual-environment-name>
```

3. activate virtual environment

* on window
``` sh
./venv/Scripts/activate
```

* on linux / mac
``` sh
source ./venv/bin/activate
```

To remove the virtual environment, first deactivate the virtual environment:

``` sh
deactivate
```
Delete its folder

* on windows:
``` sh
rm venv -Force
```

* on linux / mac:
``` sh
rm -rf venv
```

To record the virtual environment dependencies
``` sh
pip freeze > requirements.txt
```

To install all dependencies recorded in requirements.txt:
``` sh
pip install -r requirements.txt
```
