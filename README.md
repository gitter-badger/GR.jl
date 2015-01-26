# The GR module for Julia

This module provides a Julia interface to
[GR](http://gr-framework.org/), a framework for
visualisation applications.

You will need to have the GR framework installed on your
machine in order to use GR. Clone the main source using:

    git clone https://github.com/jheinen/gr

and build and install as usual with:

    cd gr
    make
    make install

This will install the GR framework into the directory ``/usr/local/gr``.

If you don't have privileges to write to the ``/usr/local`` directory,
you should install the GR framework in your home folder:

    cd gr
    make GRDIR=$HOME/gr
    make GRDIR=$HOME/gr install

Once the GR framework is installed you can use ``Pkg.add("GR")``
in Julia to install the GR module. You are now ready tu use GR.

In Julia simply type ``using GR`` and begin calling functions
in the [GR framework](http://gr-framework.org/gr.html) API.

You may also set the ``GRDIR`` environment to the GR Python module path
of an existing Anaconda (or Miniconda) installation, e.g.:

    export GRDIR=${HOME}/anaconda/lib/python2.7/site-packages/gr

