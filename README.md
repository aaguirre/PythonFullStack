PythonEnterpriseStack
=====================

Python Enterprise Stack Example

This is an example about how to build you development environment using Buildout and Pyramid

Pre-conditions:
- Latest version of setuptools must be installed. https://pypi.python.org/pypi/setuptools
  wget https://bitbucket.org/pypa/setuptools/raw/bootstrap/ez_setup.py -O - | python

Installation:
============

python bootstrap
bin/buildout

wait....


Important:
Once the buildout process is completed, in order that the example application can work fine, you need to set the email configuration on the application configuration file (development.ini) which is found under src/PyramidSite/.

After that, please reset the SQLite database running the following command.

bin/initialize_PyramidSite_db src/PyramidSite/development.ini 

Finally you can run the application executing:

bin/serve
