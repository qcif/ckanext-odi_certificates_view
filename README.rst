.. You should enable this project on travis-ci.org and coveralls.io to make
   these badges work. The necessary Travis and Coverage config files have been
   generated for you.

.. image:: https://travis-ci.org/mattRedBox/ckanext-odi_certificates_view.svg?branch=master
    :target: https://travis-ci.org/mattRedBox/ckanext-odi_certificates_view

.. image:: https://coveralls.io/repos/mattRedBox/ckanext-odi_certificates_view/badge.svg
  :target: https://coveralls.io/r/mattRedBox/ckanext-odi_certificates_view

.. image:: https://pypip.in/download/ckanext-odi_certificates_view/badge.svg
    :target: https://pypi.python.org/pypi//ckanext-odi_certificates_view/
    :alt: Downloads

.. image:: https://pypip.in/version/ckanext-odi_certificates_view/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-odi_certificates_view/
    :alt: Latest Version

.. image:: https://pypip.in/py_versions/ckanext-odi_certificates_view/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-odi_certificates_view/
    :alt: Supported Python versions

.. image:: https://pypip.in/status/ckanext-odi_certificates_view/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-odi_certificates_view/
    :alt: Development Status

.. image:: https://pypip.in/license/ckanext-odi_certificates_view/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-odi_certificates_view/
    :alt: License

=============
ckanext-odi_certificates_view
=============

A simple view renderer to display odi certificate data (usually stored with ckanext-odi_certificates_store)


------------
Requirements
------------

Tested against: Ckan API 2.7.3
Recommended to be used with ckanext-odi_certificates_store


------------
Installation
------------

.. Add any additional install steps to the list below.
   For example installing any non-Python dependencies or adding any required
   config settings.

To install ckanext-odi_certificates_view:

1. Activate your CKAN virtual environment, for example::

     . /usr/lib/ckan/default/bin/activate

2. Install the ckanext-odi_certificates_view Python package into your virtual environment (pending)::

     pip install ckanext-odi_certificates_view

3. Add ``odi_certificates_view`` to the ``ckan.plugins`` setting in your CKAN
   config file (by default the config file is located at
   ``/etc/ckan/default/production.ini``).

4. Restart CKAN. For example if you've deployed CKAN with Apache on Ubuntu::

     sudo service apache2 reload


---------------
Config Settings
---------------

Document any optional config settings here. For example::

    # The minimum number of hours to wait before re-checking a resource
    # (optional, default: 24).
    ckanext.odi_certificates_view.some_setting = some_default_value


------------------------
Development Installation
------------------------

To install ckanext-odi_certificates_view for development, activate your CKAN virtualenv and
do::

    git clone https://github.com/mattRedBox/ckanext-odi_certificates_view.git
    cd ckanext-odi_certificates_view
    python setup.py develop
    pip install -r dev-requirements.txt


-----------------
Running the Tests
-----------------

To run the tests, do::

    nosetests --nologcapture --with-pylons=test.ini

To run the tests and produce a coverage report, first make sure you have
coverage installed in your virtualenv (``pip install coverage``) then run::

    nosetests --nologcapture --with-pylons=test.ini --with-coverage --cover-package=ckanext.odi_certificates_view --cover-inclusive --cover-erase --cover-tests


---------------------------------
Registering ckanext-odi_certificates_view on PyPI
---------------------------------

ckanext-odi_certificates_view should be availabe on PyPI as
https://pypi.python.org/pypi/ckanext-odi_certificates_view. If that link doesn't work, then
you can register the project on PyPI for the first time by following these
steps:

1. Create a source distribution of the project::

     python setup.py sdist

2. Register the project::

     python setup.py register

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the first release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.1 then do::

       git tag 0.0.1
       git push --tags


----------------------------------------
Releasing a New Version of ckanext-odi_certificates_view
----------------------------------------

ckanext-odi_certificates_view is availabe on PyPI as https://pypi.python.org/pypi/ckanext-odi_certificates_view.
To publish a new version to PyPI follow these steps:

1. Update the version number in the ``setup.py`` file.
   See `PEP 440 <http://legacy.python.org/dev/peps/pep-0440/#public-version-identifiers>`_
   for how to choose version numbers.

2. Create a source distribution of the new version::

     python setup.py sdist

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the new release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.2 then do::

       git tag 0.0.2
       git push --tags
