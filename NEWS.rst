News
====

0.14 (unreleased)
-----------------
* Ignore class names starting with "Test" in "test\_" files (thanks @thisch).
* Ignore "test\_" functions only in "test\_" files.

0.13 (2017-03-06)
-----------------
* Ignore star-imported names since we cannot detect whether they are used.
* Move repository to GitHub.


0.12 (2017-01-05)
-----------------
* Detect unused imports.
* Use tokenize.open() on Python >= 3.2 for reading input files, assume
  UTF-8 encoding on older Python versions.


0.11 (2016-11-27)
-----------------
* Use the system's default encoding when reading files.
* Report syntax errors instead of aborting.


0.10 (2016-07-14)
-----------------
* Detect unused function and method arguments (issue #15).
* Detect unused \*args and \*\*kwargs parameters.
* Change license from GPL to MIT.


0.9 (2016-06-29)
----------------
* Don't flag attributes as unused if they are used as global variables
  in another module (thanks Florian Bruhin).
* Don't consider "True" and "False" variable names.
* Abort with error message when invoked on .pyc files.


0.8.1 (2015-09-28)
------------------
* Fix code for Python 3.


0.8 (2015-09-28)
----------------
* Do not flag names imported with "import as" as dead code (thanks Tom Terrace).


0.7 (2015-09-26)
----------------
* Exit with exitcode 1 if path on commandline can't be found.
* Test vulture with vulture using a whitelist module for false positives.
* Add tests that run vulture as a script.
* Add "python setup.py test" command for running tests.
* Add support for tox.
* Raise test coverage to 100%.
* Remove ez_setup.py.


0.6 (2014-09-06)
----------------
* Ignore function names starting with "test\_".
* Parse variable names in new format strings (e.g. "This is {x}".format(x="nice")).
* Only parse alphanumeric variable names in format strings and ignore types.
* Abort with exit code 1 on syntax errors.
* Support installation under Windows by using setuptools (thanks Reuben Fletcher-Costin).


0.5 (2014-05-09)
----------------
* If dead code is found, exit with 1.


0.4.1 (2013-09-17)
------------------
* Only warn if a path given on the command line cannot be found.


0.4 (2013-06-23)
----------------
* Ignore unused variables starting with an underscore.
* Show warning for syntax errors instead of aborting directly.
* Print warning if a file cannot be found.


0.3 (2012-03-19)
----------------
* Add support for python3
* Report unused attributes
* Find tuple assignments in comprehensions
* Scan files given on the command line even if they don't end with .py


0.2 (2012-03-18)
----------------
* Only format nodes in verbose mode (gives 4x speedup).


0.1 (2012-03-17)
----------------
* First release.
