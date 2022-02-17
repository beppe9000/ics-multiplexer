# ics-multiplexer
_ICS Feed Aggregation_

## What is ICS ?
Originally introduced by Apple, the iCalendar is a protocol independent standard. The ICS file format itself is defined in the [RFC-5545](https://www.rfc-editor.org/rfc/inline-errata/rfc5545.html) specification.

## What is ics-multiplexer
The purpose of this software is to group together multiple ics feeds at the same time and easily share them using a single centralized read-only url.

### Features
#### TODO
 - configuration using settings.json
 - visual pipeline configuration via browser
 - read ics from upstream urls
 - cache all events (set expiry in settings.json)
 - event filtering (allows to specify white/black lists for events)
 - event aggregation (just concatenation of the feeds for now)
 - event id rewriting for first-party management
 - duplicate checking
 - import from google calendar
 - sync from file
 - calendar viewer for all published ics feeds
 - support for past/future querying (test with google calendar to see if they pass parameters in the request)
#### DONE
 - ...

## Getting Started

1. Download the latest build, extract the archive contents in a folder of choice
2. Make a copy of `sample.settings.json` and call it `settings.json`
3. Change settings to suit your needs, save, and close your editor
4. `dotnet run`


## Web Service
### Option 1 
 The web server does the fetching and computation when invoked.
### Option 2
 The calendar is deployed as an ics file that is statically served. A background process will update the file evey once in a while.

## Web Interface
...

## Other references
https://www.webdavsystem.com/server/creating_caldav_carddav/calendar_ics_file_structure/
