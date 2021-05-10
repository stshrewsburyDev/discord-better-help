The Navigation class
====================

The Navigation class. Can be used to change the emojis used in the controls of the help menu.


Example:
--------

.. code-block:: python

    from discord.ext import commands
    from better_help import Help, Navigation

    nav = Navigation(":discord:670946129596383234", "😄", "\U0001F6D1")

    bot = commands.Bot(command_prefix="!", help_command=Help(navigation=nav))


Navigation class:
-----------------

.. py:class:: Navigation(pg_left="◀", pg_right="▶", cancel="⏹")

    Creates a navigation controls setting that can be used in the help menu.

    Accepts standard emojis in multiple ways:
        - Emoji: "👍"
        - Unicode: "\\U0001F44D"
        - Unicode Name: "\\N{THUMBS UP SIGN}"

    Using a custom emoji:
        - Discord emoji id: ":custom_emoji:8675309"

    Use ``\\\`` to get the discord representation:
        Example: ``'\\\:custom_emoji:'`` in discord

    :param str pg_left: The emoji used for the page back control of the help menu.
    :param str pg_right: The emoji used for the page forward control of the help menu.
    :param str cancel: The emoji used for the cancel control of the help menu.
