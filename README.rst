bootstrap-virtualenv
====================

This is just a simple Bash script that creates and populates a new virtualenv
for a Python project.  If the ``virtualenv`` program is not available in the
$PATH, this script downloads it from upstream and runs it locally to create the
virtualenv for the project.

Note that this is compatible with ``virtualenvwrapper``.  If a virtualenv is
active when this script is run, then it will avoid creating a new virtualenv
and attempt to install dependencies into the active environment.
