bootstrap-virtualenv
====================

This is just a simple Bash script that creates and populates a new virtualenv
for a Python project.  If the ``virtualenv`` program is not available in the
$PATH, this script downloads it from upstream and runs it locally to create the
virtualenv for the project.

Note that this is compatible with ``virtualenvwrapper``.  If a virtualenv is
active when this script is run, then it will avoid creating a new virtualenv
and attempt to install dependencies into the active environment.

Usage
-----
- Download the script::

    curl -O https://raw.github.com/fr33jc/bootstrap-virtualenv/master/bootstrap-virtualenv

- Edit the script locally and adjust the ``PROJECT_NAME`` and ``REQUIREMENTS``
  variables for your project::

    sed -i 's/example_proj/my_project_name' bootstrap-virtualenv

- Run it::

    ./bootstrap-virtualenv
