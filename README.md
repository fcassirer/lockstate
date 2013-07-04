lockstate
=========

Tools to interact with the Lockstate wifi lock web site.   Lockstate
puts out a WiFi enabled door lock.   They have a web site that enables
you to manage the lock from the site.  They report on various things
like codes, wifi level, and battery level.  The service can notify you
when someone enters and what named code was used.  Unfortunately, they do not
have an API or service that will alert you when the batter on the lock
gets low.  The level will drop from usable to not working all of a
sudden.  I got tired of getting locked out of the house ;-) I wrote a
quick hack to automatically navigate the web site and pick out the
battery level and send an email if the level gets below some preset
threshold.

This code requires the following:

- gmail account
- lockstate account
- gmail application specific password (see password & settings in your
  	gmail account to create a unique one for your app)

Note, this will probably not work if the web site changes, but for now,
I am getting an alert when the battery goes low and a running daily
log.  I have this in my crontab on my mac to run every morning at 8am.

Drop a comment in github if you find this useful.

lockstate-battery-check
