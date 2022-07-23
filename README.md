# Tips-to-create-python-package
How to create python package and link with pypi.org
create "package" folder on Desktop
create library folder "saylani-ai" in package folder (library folder can be in any name)  
come to package folder again and create "setup.py" file
write following code in "setup.py"

from setuptools import setup

setup(name = "saylani-ai",
version = "0.1"
description = "This is a Description"
long_description = "This is very very long description"
author = "Any name / your name",
packages = ["saylani-ai"],
install_packages = []
)
come to library folder "saylani-ai" and create "init.py" file. (you can write any code in init.py file)
run cmd from "package" folder and run following step by step
pip install wheel
python setup.py bdist_wheel
python setup.py sdist bdist_wheel



