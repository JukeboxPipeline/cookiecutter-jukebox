======================
cookiecutter-jukebox
======================

Cookiecutter template for a Python package in the JukeboxPipeline. See https://github.com/audreyr/cookiecutter.

I adapted the pypackage from storax a little bit.
The doc has a modified readthedocs theme already installed. There are 2 scripts that help
building the apidoc (generates rst files for your packages). The official apidoc
had a buggy formatting. Have a look at ``docs/updatedoc.py``. It is setup so that if the sphinx build is invoked,
the apidoc is generated before the actual build. This ensures that the apidoc is also built on readthedocs.
Check out the bottom of ``docs/conf.py`` if you want to alter that behavior.

* Free software: BSD license
* Pytest_ runner: Supports `unittest`, `pytest`, `nose` style tests and more
* Travis-CI_: Ready for Travis Continuous integration testing
* Tox_ testing: Setup to easily test for python 2.6, 2.7, 3.3 and PyPy_
* Sphinx_ docs: Documentation raedy for generation with, for example, ReadTheDocs_

Usage
-----

Generate a Python package project::

    cookiecutter https://github.com/JukeboxPipeline/cookiecutter-pypackage.git

Then:

* Create a repo and put it there.
* Add the repo to your Travis CI account. **Optional** 
* Add the repo to your ReadTheDocs account + turn on the ReadTheDocs service hook.
* Add the repo to coveralls
* Run `tox` to make sure all tests pass.
* Release your package the standard Python way.

Not Exactly What You Want?
--------------------------

Don't worry, you have options:

Similar Cookiecutter Templates
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* `storax/cookiecutter-pypackage`_: The original package that was slightly modified.

Fork This
~~~~~~~~~

If you have differences in your preferred setup, I encourage you to fork this
to create your own version. Once you have your fork working, add it to the
Similar Cookiecutter Templates list with a brief explanation. It's up to you
whether or not to rename your fork.

Or Submit a Pull Request
~~~~~~~~~~~~~~~~~~~~~~~~

I also accept pull requests on this, if they're small, atomic, and if they
make my own packaging experience better.


.. _Travis-CI: http://travis-ci.org/
.. _Tox: http://testrun.org/tox/
.. _Sphinx: http://sphinx-doc.org/
.. _ReadTheDocs: https://readthedocs.org/
.. _`Nekroze/cookiecutter-pypackage`: https://github.com/Nekroze/cookiecutter-pypackage
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
.. _Pytest: http://pytest.org/
.. _PyPy: http://pypy.org/
.. _Wheel: http://pythonwheels.com
