# CDL Nuxeo Code

This `README.md` is a overview of UC Regents code written at CDL to use Nuxeo.

This code is mostly written in two languages -- as of Jan 2017 python 2.7.x and node v0.10.x

Python and node both use the same `pynuxrc` configuration file format -- although the `.ini`
format based file is not 100% consistent between python and node.

As of Jan 2017; the Nuxeo version supported is Nuxeo 6.0

## [pynux](https://github.com/ucldc/pynux/)
pynux is a python wrapper for the nuxeo REST API.  It is both a library that is used
in other CDL programs and scripts; and a set of command line tools (CLI) to perform common
tasks at a command line.  Most of our tooling around metadat is based on pynx.

## [nxcli](https://github.com/ucldc/nxcli)
nx cli is a node command line based on Nuxeo's official javascript API wrapper.  I could never
figure out how to do the file upload with the REST API, but with the nuxeo javascript API I could get
upload to work.  Most bulk file uploads are done with nxcli.

## [nuxeo_spreadsheet](https://github.com/ucldc/nuxeo_spreadsheet)
Bulk metadata import tool based on google sheets.  Requires a python
environment (conda is recommended for windows)

## [nuxeo-load](https://github.com/ucldc/nuxeo-load)
Lots of miscellaneous scripts that use pynux.

## [ucldc-merritt](https://github.com/ucldc/ucldc-merritt)
Generates an atom feed for loading Nuxeo into Merritt for preservation.

## [checkcheck](https://github.com/ucldc/checkcheck)
Fixity checking for Nuxeo.  Python 3.

## [extent_stats](https://github.com/ucldc/extent_stats)
Batch reports that get run once a month.

## [fetcher for Calisphere](https://github.com/ucldc/harvester/blob/master/harvester/fetcher/nuxeofetcher.py)
"Deep harvest" of Nuxeo is coded in the UCLDC harvester.
