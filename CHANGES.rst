####################
dwdweather changelog
####################

in progress
===========

2019-10-01 0.10.0
=================
- Update library usage example, fix #15. Thanks @Lukas-Kullmann!
- Fix URI encoding woes
- Add "now" timerange for "10_minutes" resolution

2019-06-27 0.9.0
=================
- Make README.rst ASCII-clean re. #5
- Python 3.6 compatibility. Thanks, @wtfuii.
- Running two consecutive INSERT / UPDATE statements instead of a single
  UPSERT statement as the sqlite version delivered with Python does not
  support this feature. Thanks, @wtfuii.

2019-06-03 0.8.2
================
- Reestablish Python 2.7 compatibility for ``setup.py``.

2019-06-03 0.8.1
================
- Fix installation on Windows systems re. charset encoding of ``README.rst``.
  Thanks, @Noordsestern!

2019-06-03 0.8.0
================
- This and that: Fix console script entrypoint. Improve imports, debugging and inline comments.
- Adapt to changes on upstream server ftp-cdc.dwd.de
- Add ``--reset-cache`` option for dropping the cache database before performing any work
- Add ``--categories`` option for specifying list of comma-separated category names to import
- Add acquisition categories "pressure", "cloudiness" and "visibility"
- Add acquisition resolution "10_minutes"
- Improve naming of some fields for the "hourly" resolution
- Add real logging instead of verbosity printing
- Add more measurement categories
- Improve FTP error handling
- Improve SQL processing by using a single UPSERT statement instead of
  running two consecutive INSERT / UPDATE statements
- Improve ISO date parsing by switching to "dateutil"
- Modularisation and refactoring
- Make station list honor selected resolution
- Fix parsing list of categories
- Improve dataset/resolution handling
- Switch from FTP to new HTTP endpoint https://opendata.dwd.de/climate_environment/CDC/

2014-07-30 0.7.0
================
- Adapted to match modified schema for sun data

2014-07-25 0.6.0
================
- Adapted to match modified schema for wind and air temperature data

2014-07-23 0.5.0
================
- Fix a problem where verbosity was not set

2014-07-18 0.4.0
================
- Use different DWD FTP server, no longer requires FTP user authentication
- Provide access to more data ("solar")
- Reading of station data much faster due to use of specific files from DWD
- Additional fixes

2014-07-18 0.3.0
================
- Add command line client functions

2014-07-17 0.2.0
================
- First working version
- Publish to PyPI

2014-07-16 0.1.0
================
- Initial commit
