Sentry on Gondor.io
===================

Runs a Sentry instance on a gondor.io stack

Deployment notes
----------------
Requires the following environment variables be set:

* ``SENTRY_CONF`` to sentry-conf.py
* ``DJANGO_SETTINGS_MODULE`` to sentry-conf
* ``SENTRY_KEY`` a suitable secret key

To set on Gondor.io::

    gondor env:set <<label>> SENTRY_CONF=sentry-conf.py
    gondor env:set <<label>> DJANGO_SETTINGS_MODULE=sentry-conf
    gondor env:set <<label>> SENTRY_KEY=0123456789abcde
