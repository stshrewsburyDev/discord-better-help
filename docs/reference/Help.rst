The Help class
==============

The help menu class.

.. py:class:: Help(**options)

    Creates a help menu Class with your custom preference setup. (refer below for arguements)

    You can pass a range of arguements to easily change how the help command will work.
    These changes can be how information is laid out, the colour used, default titles/strings and much more.

    :param bool sort_commands: Sort commands and categories alphabetically, defaults to ``True``.
    :param bool code_block: Put the help info inside of code blocks, defaults to ``True``.
    :param bool command_list_code_block: Put command lists inside one code block, if off each command will be inside a separate code mini-block (eg: ``command1`` ``command2`` ``command3``), defaults to ``False``.
    :param bool cog_list_code_block: Put each cog in the cog list (on the index page) inside a code block, defaults to ``True``.
    :param colour: The colour to be used on the embeds, defaults to ``discord.Embed.Empty``.
    :param str no_info: The default value to put if no info can be found on something, defaults to ``No information provided``.
    :param str ending_note: Set the footer of the embed. Insert invoked prefix and command by using: (``{0}`` - Prefix used to invoke help command, ``{1}`` - Command (Commonly is "help"))
    :param str no_category: Set the name of the page with commands not part of a category, Defaults to ``No Category``.
    :param int char_limit: Set the character limit for the paginator, defaults to ``6000``.
    :param int field_limit: Set the page field limit for each page of the menu, defaults to ``15``.
    :param bool show_cooldown: Show/hide the cooldown field in command help menu's, defaults to ``True``.
    :param bool show_brief: Show/hide the brief field in command help menu's, defaults to ``False``.
    :param bool show_info_title: Changes the command description box in command help menu's to have an "Info:" title above it to match other fields, defaults to ``False``. (**Note:** enabling this will limit command descriptions to 1024 characters due to Discord API limitations)
    :param bool dm_help: DM the help menu to the author instead of show it in their channel.
    :param bool dm_help_notification: Show a message in the help request channel if ``dm_help`` is ``True``.
    :param str dm_help_message: The message to show in the DM notification, defaults to ``{0} Please check your DMs for help.``. (**Note:** Using ``{0}`` refers to the author type, for example putting ``{0.display_name}`` will show the users display name.)
    :param int timeout: Set the time (in seconds) that the menu will be active, defaults to ``30``.
    :param bool timeout_delete: Delete the help menu message on timeout, defaults to ``False``.
    :param bool timeout_remove_controls: Remove the reactions to the help menu on timeout, defaults to ``False``. (will not work if ``timeout_delete`` is set to ``True``)
    :param bool timeout_show_message: Show a message on the help menu on timeout, defaults to ``True``. (will not work if ``timeout_delete`` is set to ``True``)
    :param str timeout_message: Message to use if ``timeout_show_message`` is ``True``, defaults to ``Menu timed out.``. (will not work if ``timeout_delete`` is set to ``True``)
    :param bool closed_delete: Delete the help menu message on cancel, defaults to ``False``.
    :param bool closed_remove_controls: Remove the reactions to the help menu on cancel, defaults to ``False``. (will not work if ``closed_delete`` is set to ``True``)
    :param bool closed_show_message: Show a message on the help menu on cancel, defaults to ``True``. (will not work if ``closed_delete`` is set to ``True``)
    :param str closed_message: Message to use if ``closed_show_message`` is ``True``, defaults to ``Menu closed.``. (will not work if ``closed_delete`` is set to ``True``)


Example:
--------

.. code-block:: python

    from discord.ext import commands
    from better_help import Help

    bot = commands.Bot(command_prefix="!", help_command=Help())

