Repositories
================

Amadla Framework uses repositories for modulation of configurations.

.. note::

    With Amadla Framework you cannot throw a rock without hitting a repository!

Instead of reinventing the wheel and having to create a new package manager the usage of Git repositories was chosen. This allows for easy sharing of configurations and easy versioning of configurations.

Git already has a lot of features that are useful for configuration management. For example, you can easily revert to a previous version of a configuration if you find that the latest version is broken. You can also easily see what has changed between versions.

You also have branches and tags that allow you to have multiple versions of a configuration that can be used for different purposes. For example, you can have a development branch and a production branch. You can also have a tag for each release of your configuration.

Git is also a tool that is well known and used by many developers. This means that you can easily find people who can help you with your configuration if you get stuck.

It is also a very mature tool and with GitHub, GitLab, etc it comes with a wide range of great tools.

Amadla Framework is here to help with the management of your repositories.

Standards
---------

It is still important to note that Amadla Framework has its own standards for repositories. These standards are there to make sure that all repositories are compatible with Amadla Framework.

The standards are as follows:

Git
^^^

The repository must be a Git repository (any Git server is acceptable, you can even use multiple ones).

.. note::

    Amadla Framework does not support other version control systems for now.

Naming Convention
^^^^^^^^^^^^^^^^^

The repository must be named in the following format:

``amadla-<module type>-<what>``

* ``amadla`` is the prefix that is used to identify the repository as an Amadla Framework repository (lowercase).
* ``module type`` is the type of module that the repository contains. For example, ``apps`` or ``servers`` (lowercase).
* ``what`` is the name of the module. For example, ``nginx`` or ``wordpress`` (camel case and the first letter is uppercase).

Branches and Tags
^^^^^^^^^^^^^^^^^

The repository must have a ``master`` or ``main`` branch that contains the latest stable version of the module.

The branch convention is of Git Flow. This means that the repository must have the following branches:

* ``master`` or ``main``: The latest stable version of the module.
* ``develop``: The latest development version of the module.
* ``feature/<feature name>``: A feature branch for a new feature.
* ``release/<version>``: A release branch for a new release.
* ``hotfix/<version>``: A hotfix branch for a hotfix.
* ``bugfix/<bug name>``: A bugfix branch for a bugfix.
* ``support/<version>``: A support branch for a version that is no longer supported.
* ``experimental``: An experimental branch for experimental features.

The repository must also have a tag for each release of the module.

The tag convention is ``v<version>``.

The version must be in the following format:

``<major>.<minor>.<patch>``