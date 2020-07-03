=============================
avturl
=============================

.. image:: https://badge.fury.io/py/avturl.svg
    :target: https://badge.fury.io/py/avturl

.. image:: https://travis-ci.org/saequus/avturl.svg?branch=master
    :target: https://travis-ci.org/saequus/avturl

.. image:: https://codecov.io/gh/saequus/avturl/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/saequus/avturl

Any setting or environment variable to url

Documentation
-------------

The full documentation is at https://avturl.readthedocs.io.

Quickstart
----------

Install avturl::

    pip install avturl

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'avturl.apps.AvturlConfig',
        ...
    )

Add avturl's URL patterns:

.. code-block:: python

    from avturl import urls as avturl_urls


    urlpatterns = [
        ...
        url(r'^', include(avturl_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
