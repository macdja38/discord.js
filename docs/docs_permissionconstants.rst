.. include:: ./vars.rst

.. danger:: This documentation is for the discord.js 8.2 branch called discordv8 maintained by macdja38. You're **probably** looking for documentation on version 9 or higher, which is available on `the up-to-date, official docs site`_.

Permission Constants
====================

In discord.js, you can handle permissions in two ways. The preferred way is to just use the string name of the permission, alternatively you can use ``Discord.Constants.Permissions["permission name"]``.

--------

Valid Permission Names
----------------------

.. code-block:: js

	{
		// general
		administrator,
		createInstantInvite,
		kickMembers,
		banMembers,
		manageRoles,
		managePermissions,
		manageChannels,
		manageChannel,
		manageServer,
		changeNickname,
		manageNicknames,
		// text
		readMessages,
		sendMessages,
		sendTTSMessages,
		manageMessages,
		embedLinks,
		attachFiles,
		readMessageHistory,
		mentionEveryone,
		// voice
		voiceConnect,
		voiceSpeak,
		voiceMuteMembers,
		voiceDeafenMembers,
		voiceMoveMembers,
		voiceUseVAD
	};

Preferred Way
-------------

The preferred way of using permissions in discordv8 is to just use the name. E.g:

``role.hasPermission("voiceUseVAD")``

Alternative
-----------

You can also go the long way round and use the numerical permission like so:

``role.hasPermission( Discord.Constants.Permissions.voiceUseVAD )``