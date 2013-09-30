Badger
======

A simple personal task manager written in Python.

Usage
-----

* `badger cal` or `badger calendar` to graphically see your calendar
* `badger now` to see the current event
* `badger next` to see the next event to get ready for
* `badger assumptions` to print what badger has guessed

Settings
--------

* default view (day, week, month)

Assumptions
-----------

__missing...__

* name => filename without extension and _'s replaced with spaces
* time => badger will schedule it for you based on the following:
	* your free time
	* the event's priority
	* length - so it does not overlap other events
	* setup time - more likely to slice the event into different instances if this is low
	* ongoing - it will be fitted in repeatedly, wherever possible

Formats
-------

### Event Properties

* __name__ - full name of the event
* __time/date/when__ - when the event takes place
* __place/location/loc/where__ - where the event takes place
* __tag/type/category__ - "important" or "class" or etc.
* __priority/importance__ - low, medium, high. Or any number (relative to all others)
* __setup__ - time to get set up (warm-up time for tasks)
* __ongoing__ - "make me do this as much as possible"
* __note__ - extra textual information

### Time Formats

Things that can go in time fields. Case doesn't matter. Anything unrecognized is ignored.

#### Days of the week:

* monday tuesday wednesday thursday friday saturday sunday
* mon tue wed thur fri sat sun

#### Times:

* 10am
* 1:30pm
* 2:30 pm
* 3:30 _(am/pm guessed according to your usual work/wake hours)_ 
* four pm


