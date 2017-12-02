.. include:: ./vars.rst

.. danger:: This documentation is for the Discord.js 8.2 branch maintained by macdja38. You're **probably** looking for documentation on version 9 or higher, which is available on `the up-to-date, official docs site`_.

Invite
======

Used to represent data of an invite.

--------

Attributes
----------

maxAge
~~~~~~

`Number`, how long (in seconds) the invite has since creation before expiring.

code
~~~~

`String`, the invite code.

server
~~~~~~

The Server_ the invite is for.

channel
~~~~~~~

The ServerChannel_ the invite is for.

revoked
~~~~~~~

`Boolean`, whether the invite has been revoked or not.

createdAt
~~~~~~~~~

`Number`, timestamp of when the invite was created.

temporary
~~~~~~~~~

`Boolean`, whether the invite is temporary or not.

uses
~~~~

`Number`, uses of the invite remaining.

maxUses
~~~~~~~

`Number`, maximum uses of the invite.

inviter
~~~~~~~

User_ who sent/created the invite.

xkcd
~~~~

`Boolean`, whether the invite is intended to be easy to read and remember by a human.

--------

Functions
---------

toString()
~~~~~~~~~~

Returns the invite URL.

delete(`callback`)
~~~~~~~~~~~~~~~~~~

| **Shortcut of** ``client.deleteInvite(invite, callback)``
| **See** client.deleteInvite_

join(`callback`)
~~~~~~~~~~~~~~~~

| **Shortcut of** ``client.joinServer(invite, callback)``
| **See** client.joinServer_

.. _client.deleteInvite : ./docs_client.html#deleteinvite-invite-callback
.. _client.joinServer : ./docs_client.html#joinserver-invite-callback