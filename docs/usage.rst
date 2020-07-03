=====
Usage
=====

To use avturl in a project, add it to your `INSTALLED_APPS`:

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
