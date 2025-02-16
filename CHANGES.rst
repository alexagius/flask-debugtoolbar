Changes
=======

0.14.0 (Unreleased)
-------------------

Enhancements:

- ??

Fixes:

- ??

0.13.1 (2022-03-29)
-------------------

Fixes:

- Use a consistent version naming convention, 0.13 should have been 0.13.0 but it was yanked and you can't re-push yanked packages with the same version

0.13 (2022-03-29)
-------------------

Fixes:

- Correct `setup.cfg` to include package files by @nickjj in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/172

0.12.1 (2022-03-28)
-------------------

Fixes:

- Correct changelog and docs URLs on PyPI


0.12.0 (2022-03-28)
-------------------

Enhancements:

- Add flask.g section to show g object content. by @Yaser-Amiri in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/118
- Support gzip response by @zaw007 in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/154
- Update PyPI metadata files: add `setup.cfg` etc by @jeffwidman in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/164

Fixes:

- Remove deprecated Jinja with_ extension for Jinja 3.0 (related to Flask 2.0) by @nickjj in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/157
- Fix SQLAlchemy SELECT/EXPLAIN to use url_for to respect app prefixes.… by @mattaw in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/143
- Setup DB properly by @jeffwidman in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/148
- prefixed css classes, fixes #152 by @jnnkB in https://github.com/flask-debugtoolbar/flask-debugtoolbar/pull/153


0.11.0 (2020-02-18)
-------------------

Enhancements:

- Switch to Flask's native CLI, dropping flask_script in the process (b92391d, thanks @jeffwidman)
- Do not show DebugToolbar routes in the route map (#86, thanks @floqqi)
- Document Pygments for SQL highlighting (#127, thanks @pgiraud)

Fixes:

- Remove deprecated flask.json_available (#119, thanks @davidism)
- Remove deprecated request.is_xhr (7ce099c, thanks @jeffwidman)
- Explicitly disable `SQLALCHEMY_TRACK_MODIFICATIONS` (9c7db48, thanks @jeffwidman)
- Fix typo (#142, thanks @timgates42)


0.10.1 (2017-02-12)
-------------------

Enhancements:
- Add support for Python wheels

Fixes:

- Switch imports from deprecated flask.ext.* to flask_* syntax (#94, thanks
  Michael Lenzen & #97 thanks Iuri de Silvio)

0.10.0 (2015-04-17)
-------------------

Enhancements:

- Added new "Routes" panel displaying URL routing rules (#69, thanks Justin McKay)
- "Versions" panel displays versions of all installed packages (#49, thanks Lucas Taylor)
- SQLAlchemy displays necessary setup steps to set up query recording
- Support reformatting SQL queries if ``sqlparse`` library is available (#48, thanks Hyunjun Kim)
- Enable sorting SQLAlchemy queries (#81, thanks Eric Workman)
- Support inserting toolbar on HTML5 pages without ``</body>`` tag
- Log a warning if unable to insert the toolbar (#20, thanks Rune Halvorsen)

Fixes:

- Ensure numeric sorting of profiler "Calls" column

0.9.2 (2014-12-05)
------------------

Fixes:

- HTML escape SQL queries when syntax highlighting is not available
- Use case-insensitive comparison to normalize filenames on Windows
- Fix exception when SQL query contained non-ASCII characters

0.9.1 (2014-11-24)
------------------

Fixes:

- Fix SQL queries with byte strings on Python 3
- Fix displaying values whose `repr()` contains unprintable characters


0.9.0 (2014-01-03)
------------------

Enhancements:

- Python 3 compatibility (#54, thanks justinmayer and jmagnusson)
- Support .init_app() (#38)
- New "Config" panel displaying Flask config values (#51, thanks Alexey Diyan)
- Better PEP8-style formatting (#63, thanks Ivan Ivaschenko)

Fixes:

- Fix template editor with non-ASCII templates (#46)


0.8 (2013-02-21)
----------------

Enhancements:

- Use `itsdangerous <http://pythonhosted.org/itsdangerous/>`_ to sign SQL queries
- Expose the jQuery object as ``fldt.$`` so extensions can use the toolbar's
  copy of jQuery (#42)

Fixes:

- Don't intercept redirects on XHR requests (#41)
- Fix SQL query time display as milliseconds (#36)
- Fix ``functools.partial`` error (#35)
- Fix werkzeug request logging with logging panel (#33)
- Fix SQL panel unicode encoding error (#31)


0.7.1 (2012-05-18)
------------------

Fixes:

- loading template editor in-place over current page


0.7 (2012-05-18)
----------------

Enhancements:

- Add an in-browser template editor to the template panel
- ``DEBUG_TB_PROFILER_ENABLED`` config option to enable the profiler on all
  requests (normally it is user-enabled by clicking the checkmark)


0.6.3.1 (2012-04-16)
--------------------

New release to add missing changelog for 0.6.3


0.6.3 (2012-04-16)
------------------
Fixes:

- Compatibility with Flask-SQLAlchemy 0.16 package name


0.6.2 (2012-02-18)
------------------

Fixes:

- Installation issue on Windows with trailing slashes in MANIFEST.in

- JavaScript error when using conditional comments for ``<html>`` tag
  (like in HTML5 Boilerplate)


0.6.1 (2012-02-15)
------------------

Fixes:

- Memory leak when toolbar was enabled

- UnicodeDecodeError when request data contained binary data (e.g. session values)


Enhancements:

- ``DEBUG_TB_ENABLED`` config setting to explicitly enable or disable the toolbar

- ``DEBUG_TB_HOSTS`` config setting to enable toolbar only for specific remote hosts

- New logo for Flask instead of Django

- Monospaced font on table data

Thanks to kennethreitz and joeshaw for their contributions.


0.6 (2012-01-04)
----------------

Flask 0.8 or higher is required

Enhancements:

- Flask 0.8 compatibility

Thanks to mvantellingen
