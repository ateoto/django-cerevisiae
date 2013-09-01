Cerevisiae
============

A django app to create, modifiy and share beer recipes

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    $ pip install django-cerevisiae

To get the latest commit from GitHub

.. code-block:: bash

    $ pip install -e git+git://github.com/Ateoto/django-cerevisiae.git#egg=cerevisiae

TODO: Describe further installation steps (edit / remove the examples below):

Add ``cerevisiae`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'cerevisiae',
    )

Add the ``cerevisiae`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^cerevisiae/', include('cerevisiae.urls')),
    )

Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate cerevisiae


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    $ mkvirtualenv -p python2.7 django-cerevisiae
    $ python setup.py install
    $ pip install -r dev_requirements.txt

    $ git co -b feature_branch master
    # Implement your feature and tests
    $ git add . && git commit
    $ git push -u origin feature_branch
    # Send us a pull request for your feature branch
