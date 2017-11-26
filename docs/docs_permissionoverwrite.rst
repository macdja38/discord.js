.. include:: ./vars.rst

.. danger:: This documentation is for the discord.js 8.2 branch called discordv8 maintained by macdja38. You're **probably** looking for documentation on version 9 or higher, which is available on `the other docs site`_.

PermissionOverwrite
===================

PermissionOverwrite is used to represent data about permission overwrites for roles or users in channels.

--------

Attributes
----------

id
~~

`String`, the ID of the PermissionOverwrite. If ``overwrite.type`` is ``role``, this is the role's ID. Otherwise, it is a User_ overwrite.

type
~~~~

`String`, type of the overwrite. Either ``member`` or ``role``.

allowed
~~~~~~~

Returns the permissions explicitly allowed by the overwrite. An `Array` of Strings, which are names of permissions. More can be found at `Permission Constants`_

denied
~~~~~~

Returns the permissions explicitly denied by the overwrite. An `Array` of Strings, which are names of permissions. More can be found at `Permission Constants`_