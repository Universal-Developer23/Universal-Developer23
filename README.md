Enter Files CONNECT HTTPS



---------- Forwarded message ----------
From: Hub OS <play.github.readme@gmail.com>
Date: Wednesday, 2 February 2022
Subject: black.readthedocs@github.me
To: Program.files.c@gmail.com


Skip to content
Sign up

psf
/
black
Public
The uncompromising Python code formatter

black.readthedocs.io/en/stable/
 MIT License
 24.9k stars  1.6k forks
 Star

Notifications
Code
Issues
286
Pull requests
19
Actions
Projects
2
Wiki
Security
Insights
 main 
Go to file
Latest commit
@felix-hilden
@JelleZijlstra
felix-hilden and JelleZijlstra
…
3 hours ago
Git stats
Files
View code
README.md
Black Logo

The Uncompromising Code Formatter
Actions Status Documentation Status Coverage Status License: MIT PyPI Downloads conda-forge Code style: black

“Any color you like.”

Black is the uncompromising Python code formatter. By using it, you agree to cede control over minutiae of hand-formatting. In return, Black gives you speed, determinism, and freedom from pycodestyle nagging about formatting. You will save time and mental energy for more important matters.

Blackened code looks the same regardless of the project you're reading. Formatting becomes transparent after a while and you can focus on the content instead.

Black makes code review faster by producing the smallest diffs possible.

Try it out now using the Black Playground. Watch the PyCon 2019 talk to learn more.

Read the documentation on ReadTheDocs!

Installation and usage
Installation
Black can be installed by running pip install black. It requires Python 3.6.2+ to run. If you want to format Jupyter Notebooks, install with pip install black[jupyter].

If you can't wait for the latest hotness and want to install from GitHub, use:

pip install git+https://github.com/psf/black

Usage
To get started right away with sensible defaults:

black {source_file_or_directory}
You can run Black as a package if running it as a script doesn't work:

python -m black {source_file_or_directory}
Further information can be found in our docs:

Usage and Configuration
Black is already successfully used by many projects, small and big. Black has a comprehensive test suite, with efficient parallel tests, and our own auto formatting and parallel Continuous Integration runner. Now that we have become stable, you should not expect large formatting to changes in the future. Stylistic changes will mostly be responses to bug reports and support for new Python syntax. For more information please refer to the The Black Code Style.

Also, as a safety measure which slows down processing, Black will check that the reformatted code still produces a valid AST that is effectively equivalent to the original (see the Pragmatism section for details). If you're feeling confident, use --fast.

The Black code style
Black is a PEP 8 compliant opinionated formatter. Black reformats entire files in place. Style configuration options are deliberately limited and rarely added. It doesn't take previous formatting into account (see Pragmatism for exceptions).

Our documentation covers the current Black code style, but planned changes to it are also documented. They're both worth taking a look:

The Black Code Style: Current style
The Black Code Style: Future style
Changes to the Black code style are bound by the Stability Policy:

The Black Code Style: Stability Policy
Please refer to this document before submitting an issue. What seems like a bug might be intended behaviour.

Pragmatism
Early versions of Black used to be absolutist in some respects. They took after its initial author. This was fine at the time as it made the implementation simpler and there were not many users anyway. Not many edge cases were reported. As a mature tool, Black does make some exceptions to rules it otherwise holds.

The Black code style: Pragmatism
Please refer to this document before submitting an issue just like with the document above. What seems like a bug might be intended behaviour.

Configuration
Black is able to read project-specific default values for its command line options from a pyproject.toml file. This is especially useful for specifying custom --include and --exclude/--force-exclude/--extend-excludepatterns for your project.

You can find more details in our documentation:

The basics: Configuration via a file
And if you're looking for more general configuration documentation:

Usage and Configuration
Pro-tip: If you're asking yourself "Do I need to configure anything?" the answer is "No". Black is all about sensible defaults. Applying those defaults will have your code in compliance with many other Black formatted projects.

Used by
The following notable open-source projects trust Black with enforcing a consistent code style: pytest, tox, Pyramid, Django Channels, Hypothesis, attrs, SQLAlchemy, Poetry, PyPA applications (Warehouse, Bandersnatch, Pipenv, virtualenv), pandas, Pillow, Twisted, LocalStack, every Datadog Agent Integration, Home Assistant, Zulip, Kedro, OpenOA, FLORIS, ORBIT, WOMBAT, and many more.

The following organizations use Black: Facebook, Dropbox, KeepTruckin, Mozilla, Quora, Duolingo, QuantumBlack, Tesla.

Are we missing anyone? Let us know.

Testimonials
Mike Bayer, author of SQLAlchemy:

I can't think of any single tool in my entire programming career that has given me a bigger productivity increase by its introduction. I can now do refactorings in about 1% of the keystrokes that it would have taken me previously when we had no way for code to format itself.

Dusty Phillips, writer:

Black is opinionated so you don't have to be.

Hynek Schlawack, creator of attrs, core developer of Twisted and CPython:

An auto-formatter that doesn't suck is all I want for Xmas!

Carl Meyer, Django core developer:

At least the name is good.

Kenneth Reitz, creator of requests and pipenv:

This vastly improves the formatting of our code. Thanks a ton!

Show your style
Use the badge in your project's README.md:

[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
Using the badge in README.rst:

.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
Looks like this: Code style: black

License
MIT

Contributing
Welcome! Happy to see you willing to make the project better. You can get started by reading this:

Contributing: The basics
You can also take a look at the rest of the contributing docs or talk with the developers:

Contributing documentation
Chat on Discord
Change log
The log has become rather long. It moved to its own file.

See CHANGES.

Authors
The author list is quite long nowadays, so it lives in its own file.

See AUTHORS.md

Code of Conduct
Everyone participating in the Black project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in thePython Community Code of Conduct.

At the same time, humor is encouraged. In fact, basic familiarity with Monty Python's Flying Circus is expected. We are not savages.

And if you really need to slap somebody, do it with a fish while dancing.

Releases 19
22.1.0
Latest
4 days ago
+ 18 releases
Used by 109k
@FlorianLudwig
@randylirano
@abeituni
@sloppycoder
@MMorrison26
@Marium39hani
@competitive-programming-helper
@jplukas
+ 109,171
Contributors 303
@ambv
@JelleZijlstra
@ichard26
@hugovk
@cooperlees
@zsol
@jayaddison
@felix-hilden
@msullivan
@isidentical
@hauntsaninja
+ 292 contributors
Languages
Python
99.7%
 
Other
0.3%
© 2022 GitHub, Inc.
Terms
Privacy
