# jupyterlab-hub

JupyterLab integration for JupyterHub.

This adds a "Hub" menu to JupyterLab that allows a user to log out of JupyterHub
or access their JupyterHub control panel. This follows the JupyterLab 0.20 and
greater extension system where an extension is just an npm package, not wrapped
in a Python package.

## Prerequisites

* JupyterLab 0.22.0 or later.
* A properly configured JupyterHub.

## Installation

To install this extension into JupyterLab, do the following:

```bash
jupyter labextension install jupyterlab-hub
```

You will also need to start the single user servers in JupyterHub using the following command (that ships with JupyterLab 0.22 and greater):

```bash
jupyter labhub
```

## Development

For a development install (requires npm version 4 or later), do the following in the repository directory:

```bash
npm install
jupyter labextension link .
```

To rebuild the package and the JupyterLab app after making changes:

```bash
npm run build
jupyter lab build
```


