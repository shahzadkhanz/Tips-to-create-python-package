# Tips-to-create-python-package
How to create python package and link with pypi.org

1 - Create "package" folder on Desktop

2 - Create library folder "saylani-ai" in package folder (library folder can be in any name)  

3 - Come to package folder again and create "setup.py" file

4 - Write following code in "setup.py"

from setuptools import setup

setup(name = "saylani-ai",

version = "0.1"

description = "This is a Package"

long_description = "This is very very long description"

author = "Any name / your name",

packages = ["saylani-ai"],

install_packages = []

)

5 - Come to library folder "saylani-ai" and create "init.py" file. (you can write any code in init.py file)

6 -  Run cmd from "package" folder and run following step by step

### pip install wheel

### python setup.py bdist_wheel

### python setup.py sdist bdist_wheel

7 - After runing all above there will be 2 folder created automatically in "package" folder

8 - Run following command after every update in .py file

### python setup.py sdist bdist_wheel

### 9 -  Setup an account on https://pypi.org

10 - For publishing the package on pypi.org run following command

### pip install twine

### twine upload dist/*

Now Enter User Name and Pass of pypi account

11 - Package has been uploaded


