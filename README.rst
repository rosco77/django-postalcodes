Django Postal Codes
===================

A simple data model for storing postal codes with placenames and location.

Installing
----------

You can clone the repository and install from source::

    python setup.py install

or use `pip` to install from PyPI::

    pip install django-postalcodes

.. note::
    Version 0.2+ requires a GIS backend (e.g. PostGIS). Migrating from 0.1 will
    not be straightforward if you have existing data decimal data or do not
    have a GIS backend.

If you are using South you must use South >= 1.0 to ensure compatability with
the new `south_migrations` migrations module name.

Getting data
------------

Postal code data is available from a number of sources.  There is a built in management command to now update global postcodes from the following OpenData resource(http://download.geonames.org/export/zip/).

To install postcode data download the zip file from the above link and run the following command
