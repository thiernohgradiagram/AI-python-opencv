# AI-python-opencv
Artificial Intelligence project with python and opencv

echo $PATH | tr ':' '\n' | grep 'Python'	-> list the path of the scripts and executables for all installed python versions
python --version 				-> list the current python version

# py is the python launcher available for windows
# py is used to select the python interpreter (python.exe) to load in the console.
# By default, it will always select the latest python interpreter. 
# py is also used to select the python interpreter (python.exe) to use when running a python script.
py						-> launch the latest python interpreter (python.exe) available in your system
py -3.7						-> launch the python interpreter (python.exe) version 3.7 to the console
py -3.12 hello.py				-> execute the hello script using the python interpreter (python.exe) version 3.12
py --list | py -0				-> list all python versions

pip install pyserial && pip freeze > requirements.txt		-> install pyserial in the current python version (the first python found in the path)
pip3.9 install pyserial && pip freeze > requirements.txt  	-> install pyserial in python version 3.9

Python Virtual Environments are sanboxes where we can use python and 
install libraries and packages without installing them in our main python installations
This allows us to not corrupt and create issues with our main python installations
This isolation allows you to work on multiple Python projects with different dependencies without worrying about conflicts between libraries or versions.
Each virtual environment maintains its own set of installed packages, separate from the global Python installation and other virtual environments.
your Python virtual environment should still work even if you delete your Python installation. This is because the virtual environment contains its own copy of the Python interpreter and necessary libraries, which are independent of the global Python installation on your system.
When you create a virtual environment, it copies the necessary files from your Python installation into the virtual environment directory. This includes the Python interpreter executable and standard library modules. As long as these files remain intact within the virtual environment directory, you can continue to use the virtual environment even if the global Python installation is removed.

py -3.7 -m venv myvenv  -> creating a python3.7 virtual environment named myvenv using the windows python luncher
python -m venv myvenv   -> creating a python virtual environment named myvenv using the current python.exe
myvenv/scripts/activate				-> activating the python virtual environment.
myvenv/scripts/deactivate			-> deactivating the python virtual environment.

