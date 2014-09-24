[![Build Status](https://travis-ci.org/FalconSocial/pre-commit-python-sorter.svg?branch=master)](https://travis-ci.org/FalconSocial/pre-commit-python-sorter)
[![Coverage Status](https://img.shields.io/coveralls/FalconSocial/pre-commit-python-sorter.svg)](https://coveralls.io/r/FalconSocial/pre-commit-python-sorter)


Pre-commit python module sorter
===============================

This is a [pre-commit](https://github.com/pre-commit) hook that will sort your imports for you (or show you how it should be done).

* [pre-commit](https://github.com/pre-commit)
* [isort](https://github.com/timothycrosley/isort)


Add this to your ``.pre-commit-config.yaml`` file

    - repo: git@github.com:FalconSocial/pre-commit-python-sorter.git
      sha: 0.0.2
      hooks:
      - id: python-import-sorter
        args: ['--diff-only']  # Will show only the diff and let you know that something is up

Development: ``pip install -r requirements-dev.txt``
Testing: ``py.test --cov pre_commit_hook tests/``
