Changelog
=========

Release 0.4.1
-------------

- Rename ``find_request_handler`` to ``find_route``.
- Rename some internal variables, notably all references to ``handler`` that
  were actually a ``Route`` instance have been renamed to route.
- Minor fixes.

Release 0.4.0
-------------

- Implemented redirection relative to Application's root. See issue #1 on github: https://github.com/pyroutes/pyroutes/issues/1
- Fixed argument defaults being overwritten. See issue #5 on github: https://github.com/pyroutes/pyroutes/issues/3
- Altered logic for matching routes (stricter matching of argument count)
- Code simplification on many minor details
- Some minor regressions introduced by the middleware fixed

Release 0.3.1
-------------

- Remove leftover print statement causing errors using mod_wsgi

Release 0.3.0
-------------

- Added support for autopopulating handler method with data from the URL.
- Added middleware support
- New and improved documentation
- Lots of cleanups on the code.

Release 0.2.2
-------------

- Fixed bug where setting the TEMPLATE_DIR-option in ``pyroutes_settings.py``
  would cause the default 404,403 and 400 error pages to not work.
- Fix bug where pyroutes would add two content-type headers to responses. (Thanks to Dalton Barreto)
- Fixed IF_MODIFIED_SINCE handling in utils.fileserver on windows.

Release 0.2.1
-------------

- Reduce setup.py dependencies to only distutils.
- Fix packaging of default templates
- Fix pypi-package complaining about README file missing.
- Fix unstable cookie handling in some cornercases.

Release 0.2.0
-------------

- New Request object included to every route. *Backward incompatible*
- New cookie handling framework
- Automatic HTTP-status code lookups in Response-objects.
- Project settings
- Better debug-pages when DEBUG=True in settings.
- Development fileserver
- Development autoreloader

