===================
restrict-ip-country
===================

`restrict-ip-country` is a reusable Django app for restricting ip addresses and country areas from accessing site.

Contents:

.. toctree::

    install
    usage
    settings


Configure GeoIP2 settings
===========================

Ensure you setup `GeoIP2`, read more here: https://docs.djangoproject.com/en/3.2/ref/contrib/gis/geoip2/
global variables in your ``settings.py``::

    GEOIP_PATH=os.path.join(BASE_DIR, 'data')

A string or pathlib.Path specifying the directory where the GeoIP data files are located. 
This setting is required.

    GEOIP_CITY='GeoLite2-City.mmdb'

The basename to use for the GeoIP city data file. Defaults to `GeoLite2-City.mmdb`, 
download here: https://git.io/GeoLite2-City.mmdb.
