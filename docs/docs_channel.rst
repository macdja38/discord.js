.. include:: ./vars.rst

.. danger:: This documentation is for the Discord.js 8.2 branch maintained by macdja38. You're **probably** looking for documentation on version 9 or higher, which is available on `the up-to-date, official docs site`_.

Channel
=======

**extends** Equality_

The Channel class is the base class for all types of channel.

--------

Attributes
----------

id
~~

The ID of the channel, a `String`.

client
~~~~~~

The Client_ that cached the channel.

isPrivate
~~~~~~~~~

Indicates whether the channel is PM channel, is `Boolean`.

createdAt
~~~~~~~~~

A `Date` referring to when the channel was created.

--------

Functions
---------

delete()
~~~~~~~~~~~~~~~

Deletes the channel.