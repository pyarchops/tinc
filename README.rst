=====================
pyArchOps/tinc
=====================


.. image:: https://badge.fury.io/py/pyarchops-tinc.svg
        :target: https://pypi.python.org/pypi/pyarchops-tinc

.. image:: https://img.shields.io/gitlab/pipeline/pyarchops/tinc/next-release.svg
        :target: https://gitlab.com/pyarchops/tinc/pipelines

.. image:: https://readthedocs.org/projects/pyarch-tinc/badge/?version=latest
        :target: https://pyarch-tinc.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status

.. image:: https://pyup.io/repos/github/pyarchops/tinc/shield.svg
     :target: https://pyup.io/repos/github/pyarchops/tinc/
          :alt: Updates


tinc


* Free software: MIT license
* Documentation: https://pyarchops-tinc.readthedocs.io.


Features
--------

* tinc

Instalation
--------------

.. code-block:: console

    $ pip install pyarchops-tinc


Usage
--------

.. code-block:: python

    import os
    import pyarchops_tinc

    api = Api(
        '127.0.0.1:22',
        connection='smart',
        remote_user='ubuntu',
        private_key_file=os.getenv('HOME') + '/.ssh/id_rsa',
        become=True,
        become_user='root',
        sudo=True,
        ssh_extra_args='-o StrictHostKeyChecking=no'
    )
    result = pyarchops_tinc.apply(api)
    print(result)

Development
-----------

Install requirements:

.. code-block:: console

    $ sudo pacman -S tmux python-virtualenv python-pip libjpeg-turbo gcc make vim git tk tcl

Git clone this repository

.. code-block:: console

    $ git clone https://github.com/pyarchops/tinc.git pyarchops.tinc
    $ cd pyarchops.tinc


2. See the `Makefile`, to get started simply execute:

.. code-block:: console

    $ make up


Credits
-------

* TODO

