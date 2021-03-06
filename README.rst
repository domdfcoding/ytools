########
ytools3
########

.. start short_desc

**Library for validating yaml files against schema and selectively dumping nodes from yaml (or json) documents in yaml or json format.**

.. end short_desc

This is a port of the Python 2-only ``ytools`` ( https://github.com/yaccob/ytools ) to Python 3.

.. start shields

.. list-table::
	:stub-columns: 1
	:widths: 10 90

	* - Docs
	  - |docs| |docs_check|
	* - Tests
	  - |actions_linux| |actions_windows| |actions_macos| |coveralls|
	* - PyPI
	  - |pypi-version| |supported-versions| |supported-implementations| |wheel|
	* - Activity
	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
	* - QA
	  - |codefactor| |actions_flake8| |actions_mypy| |pre_commit_ci|
	* - Other
	  - |license| |language| |requires|

.. |docs| image:: https://img.shields.io/readthedocs/ytools3/latest?logo=read-the-docs
	:target: https://ytools3.readthedocs.io/en/latest
	:alt: Documentation Build Status

.. |docs_check| image:: https://github.com/domdfcoding/ytools3/workflows/Docs%20Check/badge.svg
	:target: https://github.com/domdfcoding/ytools3/actions?query=workflow%3A%22Docs+Check%22
	:alt: Docs Check Status

.. |actions_linux| image:: https://github.com/domdfcoding/ytools3/workflows/Linux/badge.svg
	:target: https://github.com/domdfcoding/ytools3/actions?query=workflow%3A%22Linux%22
	:alt: Linux Test Status

.. |actions_windows| image:: https://github.com/domdfcoding/ytools3/workflows/Windows/badge.svg
	:target: https://github.com/domdfcoding/ytools3/actions?query=workflow%3A%22Windows%22
	:alt: Windows Test Status

.. |actions_macos| image:: https://github.com/domdfcoding/ytools3/workflows/macOS/badge.svg
	:target: https://github.com/domdfcoding/ytools3/actions?query=workflow%3A%22macOS%22
	:alt: macOS Test Status

.. |actions_flake8| image:: https://github.com/domdfcoding/ytools3/workflows/Flake8/badge.svg
	:target: https://github.com/domdfcoding/ytools3/actions?query=workflow%3A%22Flake8%22
	:alt: Flake8 Status

.. |actions_mypy| image:: https://github.com/domdfcoding/ytools3/workflows/mypy/badge.svg
	:target: https://github.com/domdfcoding/ytools3/actions?query=workflow%3A%22mypy%22
	:alt: mypy status

.. |requires| image:: https://requires.io/github/domdfcoding/ytools3/requirements.svg?branch=master
	:target: https://requires.io/github/domdfcoding/ytools3/requirements/?branch=master
	:alt: Requirements Status

.. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/ytools3/master?logo=coveralls
	:target: https://coveralls.io/github/domdfcoding/ytools3?branch=master
	:alt: Coverage

.. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/ytools3?logo=codefactor
	:target: https://www.codefactor.io/repository/github/domdfcoding/ytools3
	:alt: CodeFactor Grade

.. |pypi-version| image:: https://img.shields.io/pypi/v/ytools3
	:target: https://pypi.org/project/ytools3/
	:alt: PyPI - Package Version

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/ytools3?logo=python&logoColor=white
	:target: https://pypi.org/project/ytools3/
	:alt: PyPI - Supported Python Versions

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/ytools3
	:target: https://pypi.org/project/ytools3/
	:alt: PyPI - Supported Implementations

.. |wheel| image:: https://img.shields.io/pypi/wheel/ytools3
	:target: https://pypi.org/project/ytools3/
	:alt: PyPI - Wheel

.. |license| image:: https://img.shields.io/github/license/domdfcoding/ytools3
	:target: https://github.com/domdfcoding/ytools3/blob/master/LICENSE
	:alt: License

.. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/ytools3
	:alt: GitHub top language

.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/ytools3/v3.0.1
	:target: https://github.com/domdfcoding/ytools3/pulse
	:alt: GitHub commits since tagged version

.. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/ytools3
	:target: https://github.com/domdfcoding/ytools3/commit/master
	:alt: GitHub last commit

.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
	:alt: Maintenance

.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/ytools3
	:target: https://pypi.org/project/ytools3/
	:alt: PyPI - Downloads

.. |pre_commit_ci| image:: https://results.pre-commit.ci/badge/github/domdfcoding/ytools3/master.svg
	:target: https://results.pre-commit.ci/latest/github/domdfcoding/ytools3/master
	:alt: pre-commit.ci status

.. end shields


Features
---------

* Output ``yaml`` as ``json`` or ``python``

* Output ``json`` as ``yaml`` or ``python`` (provided that there are no duplicate mapping entry in the ``json`` source)

* Extract particular nodes from ``yaml`` and ``json`` files.

	+ If ``yaml`` is used as output format (default) the output is a valid ``yaml`` document.

* Validate ``yaml`` and ``json`` documents.

	+ The ``json-schema`` can be provided in ``yaml`` format as well, which improves readability and writability.

* Preserve order of mapping-keys in ``yaml`` and ``json`` output.

* Multi-document support

	+ Multiple input files

		- ... as well as multiple ``yaml`` documents within a file
		- ... and a combination of both


Installation
--------------

.. start installation

``ytools3`` can be installed from PyPI.

To install with ``pip``:

.. code-block:: bash

	$ python -m pip install ytools3

.. end installation
