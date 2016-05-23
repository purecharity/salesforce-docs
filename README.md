# Salesforce Pure Charity App Documentation

This is the documentation repository for the Pure Charity App for Salesforce.

The latest version available can always be found [here](http://salesforceinstall.purecharity.com).

You can also all take a look at the [Changelog file](CHANGELOG.md) and see what changed from version to version.

## How does it work?

This website is running on [MkDocs](http://www.mkdocs.org), a fast, simple and downright gorgeous static site generator that's geared towards building project documentation.

## Installation

In order to install MkDocs you'll need Python installed on your system, as well as the Python package manager, pip. You can check if you have these already installed like so:

```bash
$ python --version
Python 2.7.2
$ pip --version
pip 1.5.2
```

MkDocs supports Python 2.6, 2.7, 3.3, 3.4 and 3.5.

On Windows we recommend that you install Python and pip with Chocolatey.

Install the mkdocs package using pip:

pip install mkdocs
You should now have the mkdocs command installed on your system. Run mkdocs --version to check that everything worked okay.

```bash
$ mkdocs --version
mkdocs, version 0.15.2
```

## Running

MkDocs comes with a built-in webserver that lets you preview your documentation as you work on it. We start the webserver by making sure we're in the same directory as the mkdocs.yml config file, and then running the mkdocs serve command:

```bash
$ mkdocs serve
Running at: http://127.0.0.1:8000/
```

## Deploying

```bash
$ mkdocs gh-deploy --clean
```
