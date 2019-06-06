Redash-Iodide
===========

`Redash <https://redash.io>`_ extensions for
`Iodide <https://github.com/iodide-project/iodide>`_.

.. image:: https://circleci.com/gh/mozilla/redash-iodide.svg?style=svg
    :target: https://circleci.com/gh/mozilla/redash-iodide

.. image:: https://codecov.io/gh/mozilla/redash-iodide/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/mozilla/redash-iodide

.. image:: https://img.shields.io/badge/calver-YYYY.M.PATCH-22bfda.svg
   :target: https://calver.org/
   :alt: CalVer - Timely Software Versioning

Installation
------------

Please install the package using your favorite package installer::

    pip install redash-iodide

Development
-----------

During the development we're providing some convenience Make tasks that are
supposed to be run from the Docker host machine, not from inside a container.

Create the database
~~~~~~~~~~~~~~~~~~~

Only once please::

    make database

Install NPM modules
~~~~~~~~~~~~~~~~~~~

First install the Node modules::

    make node_modules

Start the containers
~~~~~~~~~~~~~~~~~~~~

Start backend, Celery, Redis, Postgres::

    make up

Run webpack devserver
~~~~~~~~~~~~~~~~~~~~~

Please run in parallel to the containers above::

    make devserver

Start shell
~~~~~~~~~~~

To enter the container and run a bash shell run::

    make bash

Run tests
~~~~~~~~~

To run the tests (from the host machine) run::

    make test

Issues & questions
------------------

See the `issue tracker on GitHub <https://github.com/mozilla/redash_iodide/issues>`_
to open tickets if you have issues or questions about Redash_Iodide.

