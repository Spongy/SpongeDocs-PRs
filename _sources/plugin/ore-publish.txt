======================
Publishing Your Plugin
======================

Sponge's official plugin / mod repository, `Ore <http://ore-staging.spongepowered.org>`_, is a free and open-source
project that anyone may publish their Sponge plugins or Forge mods on.

Packaging Your Plugin
~~~~~~~~~~~~~~~~~~~~~

Ore requires any projects to be packaged with a ``mcmod.info`` descriptor file in the top-level of your JAR file. This
file is used to automatically infer some important details about your project to make the upload process easier. Ore
will reject your plugin if this file is missing from the JAR. Luckily, Sponge API has a built in annotation processor
that creates this file for you automatically, on compile, using the ``@Plugin`` annotation that you have likely
already created in your plugin's main class.

.. note::

    For more information on creating and compiling your first plugin, see :doc:`/plugin/plugin-class`

For reference, here is a sample ``mcmod.info`` file:

.. code-block:: json

    [
        {
            "modid": "my-plugin",
            "name": "MyPlugin",
            "version": "1.0.0",
            "description": "My first plugin!",
            "url": "https://spongepowered.org",
            "authorList": [
                "windy",
                "Zidane",
                "gabizou"
            ],
            "requiredMods": [
                "bookotd@1.0.0",
                "ore-test@1.0.0",
                "worldedit@1.0.0"
            ],
            "dependencies": [
                "bookotd@1.0.0",
                "ore-test@1.0.0",
                "worldedit@1.0.0"
            ]
        }
    ]

At the very least, each Ore project *must* have the ``modid``, ``name`` and, ``version`` fields completed.

Uploading Your Plugin
~~~~~~~~~~~~~~~~~~~~~

Once your plugin's JAR file is packaged with an ``mcmod.info`` descriptor file in the top-level, your plugin is ready
for uploading! To create a project on Ore, you must have an account on
`Sponge Forums <https://forums.spongepowered.org>`_. Hitting the "Sign up" button in the top-right corner will take
you to the appropriate page to create one. If you already have an account, just hit the "Log in" button in the
top-right corner to log into Ore.

Once logged in, navigate to your avatar and select the "New" option in the drop-down menu that appears, or just press
the "C" key.

Setting Up Your Project on Ore
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

After uploading your plugin, you will be presented with some settings to configure your project however you like. Don't
worry, all of these can be changed later in the settings panel. After setting up your project you will be able to invite
Sponge users to be a part of your project. Any user that is registered on the forums can be invited to a project even if
they have never logged onto Ore. Upon creation of your project, the users you have invited will receive a notification
and will be able to either accept or decline your invitation. Project members will not be visible to the public until
the invitation has been accepted.

There are currently three groups you may assign to project members: `Developer`, `Editor`, and `Support`. The user
who created the project will be assigned the `Owner` which has unrestricted access to the project. Here is a quick
rundown of what each group can do within your project.

Developers
----------

Developers may create/edit release channels, pages and create/edit versions.

Editor
------

Editors may edit pages.

Support
-------

Support cannot do anything, merely a way of showing that the member is a part of the project.
