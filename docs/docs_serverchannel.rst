.. include:: ./vars.rst

.. danger:: This documentation is for the Discord.js 8.2 branch maintained by macdja38. You're **probably** looking for documentation on version 9 or higher, which is available on `the up-to-date, official docs site`_.

ServerChannel
=============

**extends** Channel_

A ServerChannel is a Channel_ that belongs to a Server_.

--------

Attributes
----------

name
~~~~

`String`, name of the channel.

type
~~~~

`String`, either ``voice`` or ``text``.

position
~~~~~~~~

`Number`, position in the channel list.

permissionOverwrites
~~~~~~~~~~~~~~~~~~~~

Cache_ of all the PermissionOverwrite_ objects affecting the channel.

server
~~~~~~

Server_ the channel belongs to.

Functions
---------

permissionsOf(userOrRole)
~~~~~~~~~~~~~~~~~~~

**Aliases:** permsOf

Returns a ChannelPermissions_ object of a user or role's permissions in that channel.

mention()
~~~~~~~~~

Returns a `string` that can be used in discord messages to mention a channel. `serverChannel.toString()` defaults to this.

update(data, `callback`)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

| **Shortcut of** ``client.updateChannel(channel, data, callback)``
| **See** client.updateChannel_
