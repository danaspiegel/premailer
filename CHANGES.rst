premailer Changes
=================

Peter's note: Unfortunately, ``premailer`` has never kept a change log. But it's
never too late to start, so let's start here and now.

3.7.0
-----

* Drop support for Python 2.7 and 3.4. Add test support for 3.8

3.6.2
-----

* Don't strip ``!important`` on stylesheets that are ignored
  See https://github.com/peterbe/premailer/pull/242
  Thanks @nshenkman

3.6.1
-----

* The ``disable_validation`` wasn't passed to ``csstest_to_pairs``
  See https://github.com/peterbe/premailer/pull/235
  Thanks @mbenedettini

3.6.0
-----

* Add ``allow_insecure_ssl`` option for external URLs

3.5.0
-----

* Change default ``cachetools`` implementation to ``cachetools.LFUCache``.

* Now possible to change ``cachetools`` implementation with environment variables.
  See README.rst.

* To avoid thread unsafe execution, the function caching decorator now employs a lock.
  See https://github.com/peterbe/premailer/issues/225
