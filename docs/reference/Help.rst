The Help class
==============

The help menu class.


Example:
--------

.. code-block:: python

    from discord.ext import commands
    from better_help import Help

    bot = commands.Bot(command_prefix="!", help_command=Help())


Customisation:
--------------

You can pass a range of arguements to easily change how the help command will work.

These changes can be how information is laid out, the colour used, default titles/strings and much more.


The basics:
^^^^^^^^^^^

``sort_commands`` - Sort commands and categories alphabetically.

``code_block`` - Put the help info inside of code blocks, defaults to ``True``.

``command_list_code_block`` - Put command lists inside one code block, if off each command will be inside a separate code mini-block (eg: ``command1`` ``command2`` ``command3``), defaults to ``False``.

``cog_list_code_block`` - Put each cog in the cog list (on the index page) inside a code block, defaults to ``True``.

``colour`` - The colour to be used on the embeds, defaults to ``discord.Embed.Empty``.

``no_info`` - The default value to put if no info can be found on something, defaults to ``No information provided``.

``ending_note`` - Set the footer of the embed.

``no_category`` - Set the name of the page with commands not part of a category, Defaults to ``No Category``.

``char_limit`` - Set the character limit for the paginator, defaults to ``6000``.

``field_limit`` - Set the page field limit for each page of the menu, defaults to ``15``.


DM help setup:
^^^^^^^^^^^^^^

``dm_help`` - DM the help menu to the author instead of show it in their channel.

``dm_help_notification`` - Show a message in the help request channel if ``dm_help`` is ``True``.

``dm_help_message`` - The message to show in the DM notification, defaults to ``{0} Please check your DMs for help.``.

**Note:** Using ``{0}`` in ``dm_help_message`` refers to the author type, for example putting ``{0.display_name}`` will show the users display name.


Configuring the timeout:
^^^^^^^^^^^^^^^^^^^^^^^^

``timeout`` - Set the time (in seconds) that the menu will be active, defaults to ``30``.

``timeout_delete`` - Delete the help menu message on timeout, defaults to ``False``.

``timeout_remove_controls`` - Remove the reactions to the help menu on timeout, defaults to ``False``.

``timeout_show_message`` - Show a message on the help menu on timeout, defaults to ``True``.

``timeout_message`` - Message to use if ``timeout_show_message`` is ``True``, defaults to ``Menu timed out.``.

**Note:** ``timeout_remove_controls``, ``timeout_show_message`` and ``timeout_message`` will not work if ``timeout_delete`` is set to ``True``.


Configuring the cancel button:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``closed_delete`` - Delete the help menu message on cancel, defaults to ``False``.

``closed_remove_controls`` - Remove the reactions to the help menu on cancel, defaults to ``False``.

``closed_show_message`` - Show a message on the help menu on cancel, defaults to ``True``.

``closed_message`` - Message to use if ``closed_show_message`` is ``True``, defaults to ``Menu closed.``.

**Note:** ``closed_remove_controls``, ``closed_show_message`` and ``closed_message`` will not work if ``closed_delete`` is set to ``True``.
