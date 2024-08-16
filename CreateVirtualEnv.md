1. cd to the folder where you want to store this virtural environment for this specific project e.g.
   pc:  ```c:/dev/jobfindchatbot``` 
   mac: ```~/dev/jobfindchatbot``` 
2. create virtual environment

``` sh
python -m venv venv
```

3. activate virtual environment

* os window
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