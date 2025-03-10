Customize your Channels experience
==================================

|all-plans| |cloud| |self-hosted|

.. |all-plans| image:: ../images/all-plans-badge.png
  :scale: 30
  :target: https://mattermost.com/pricing
  :alt: Available in Mattermost Free and Starter subscription plans.

.. |cloud| image:: ../images/cloud-badge.png
  :scale: 30
  :target: https://mattermost.com/sign-up
  :alt: Available for Mattermost Cloud deployments.

.. |self-hosted| image:: ../images/self-hosted-badge.png
  :scale: 30
  :target: https://mattermost.com/deploy
  :alt: Available for Mattermost Self-Hosted deployments.

You can customize your Channels experience in the following ways in **Settings**:

- `Notifications <#notifications>`__
- `Display <#display>`__
- `Sidebar <#sidebar>`__
- `Advanced <#advanced>`__

.. tabs::

  .. tab:: Mattermost v6.0 onwards

      In Mattermost v6.0, **Account Settings** have moved.

      - Access **Profile** and **Security** settings from your avatar in the Global Header.
      - Access **Notifications**, **Display**, **Sidebar**, and **Advanced Settings** by selecting the gear |gear-icon| icon in the Global Header.

      .. |gear-icon| image:: ../images/settings-outline_F08BB.svg
        :alt: Select the gear icon to open the Settings dialog.

  .. tab:: Mattermost v5.39 and earlier

      In Mattermost versions up to v5.39, access all of your user settings in **Account Settings** from the **Main Menu** by selecting the three horizontal lines (also known as a hambuger menu) at the top of the channel sidebar.

Notifications
-------------

Settings to configure desktop notifications, desktop notification sounds, email notifications, mobile push notifications, and words that trigger mentions.

Desktop notifications
~~~~~~~~~~~~~~~~~~~~~

Desktop notifications appear in the top corner of your main monitor when there is activity in Mattermost.

Send desktop notifications
^^^^^^^^^^^^^^^^^^^^^^^^^^

Choose what activity triggers a desktop notification. This setting applies globally, but this preference is customizable for each channel from the channel name drop-down menu. Desktop notifications are available on Chrome, Edge, Firefox, and Safari.

When `desktop app <https://mattermost.com/apps>`__ notifications are set to "Only for mentions and direct messages":

- An empty red circle is displayed over the upper right corner of the Mattermost dock icon when any message without an at-mention is received. 
- A solid red circle with a post count is displayed when a message with an at-mention is received.
- And when `Collapsed Reply Threads <https://docs.mattermost.com/channels/organize-conversations.html>`__ is enabled, you can choose to receive desktop notifications about `threads you're following <https://docs.mattermost.com/channels/organize-conversations.html#start-or-reply-to-threads>`__.

Notification sound
^^^^^^^^^^^^^^^^^^

Notification sounds fire for any activity that would trigger a desktop notification. Notification sounds are available on Chrome, Edge, Firefox, and Safari in addition to the Mattermost Desktop App.

Email notifications
~~~~~~~~~~~~~~~~~~~

Email notifications are sent for mentions and direct messages after you’ve been offline for more than 60 seconds or away from Mattermost for more than five minutes. Change the email where notifications are sent by selecting **Profile > Profile Settings > Email**.

If your System Admin has enabled `email batching <https://docs.mattermost.com/configure/configuration-settings.html#enable-email-batching>`__, you'll have additional options under this settings to select how often email notifications will be sent. All notifications received over this time period are combined and sent in a single email.

Mobile push notifications
~~~~~~~~~~~~~~~~~~~~~~~~~

Push notifications can be sent to your mobile device if you have the Android or iOS app installed. You can choose the type of activity that will send a notification.

By default, push notifications are sent **For mentions and direct messages**. If push notifications are sent **Never**, the Mattermost setting to trigger push notifications depending on your `Mattermost availability <https://docs.mattermost.com/welcome/set-your-status-availability.html>`__ is hidden. If your System Admin hasn't set up push notifications, this setting will be disabled.

If you're actively viewing a channel (public or private), direct message, or group message using the Desktop App or a browser, no push notifications will be sent for that channel. If a notification is viewed using the Desktop App or a browser, the lockscreen notification will clear on Android, and on iOS the badge on the Mattermost app icon will count down accordingly.

Browser tab notifications
~~~~~~~~~~~~~~~~~~~~~~~~~

If Mattermost is open in a browser tab, the favicon updates to notify you of unread messages (\*) and a count of mentions or direct messages. Browser tab notifications are available on Chrome, Edge, Firefox, and Safari.

.. image:: ../images/browser_notification.png

Trigger mobile push notifications when
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can also choose when to send push notifications depending on your Mattermost availability. By default, push notifications are sent if your availability is **Away** or **Offline**. If **Send Mobile Push Notifications** is set as **Never**, this setting is hidden. If your System Admin has not set up push notifications, this setting will be disabled.

Words that trigger mentions
~~~~~~~~~~~~~~~~~~~~~~~~~~~

By default, you receive notifications when someone posts a message that contains your non-case sensitive username or @username. You also receive notifications when someone uses the @channel, @all, and @here mentions. You can customize the words that trigger mentions by typing them into the input box. This is useful if you want to be notified of all posts on a certain topic, for example, "marketing".

Reply notifications
~~~~~~~~~~~~~~~~~~~

When `Collapsed Reply Threads <https://docs.mattermost.com/channels/organize-conversations.html>`__ is disabled, you can choose to receive mention notifications when someone replies to a thread you have started or have participated in.

- You're considered to start a thread when you post a message to which other members of your team reply.
- You're considered to be a participant in a thread when you post a message using the `reply button <https://docs.mattermost.com/channels/reply-to-messages.html>`__ in an pre-existing thread.

.. note::
  This setting is hidden when Collapsed Reply Threads is enabled.

Automatic direct message replies
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Set an automated custom message that will be sent once per day in response to direct messages. Mentions in public and private channels won't trigger the automated reply. Enabling Automatic Replies sets your availability to **Out of Office** and disables desktop, email, and push notifications. This setting is experimental and `must be enabled by your System Admin <https://docs.mattermost.com/configure/configuration-settings.html#enable-automatic-replies>`__.

Display
-------

Settings to configure clock and teammate name display preferences.

Theme
~~~~~

Select **Theme Colors** to select from four standard themes designed by the Mattermost team. To make custom adjustments on the four standard theme colours, select a standard theme and then select **Custom Theme** to load the standard theme into the custom theme color selectors.

Select **Custom Theme** to customize your theme colors and share them with others by copying and pasting theme vectors into the input box. Observe a live preview as you customize theme colors, then select **Save** to confirm your changes. Discard your changes by selecting **Cancel**, or by exiting the settings modal and selecting **Yes, Discard**.

In Enterprise edition, if you belong to multiple teams, you can optionally select the checkbox **Apply new theme to all my teams** to have the theme show up across teams. Otherwise, the changes will only apply to the current team.

Learn more about the custom theme color selectors `here <https://docs.mattermost.com/welcome/customize-your-theme.html>`__.

Select **Import theme colors from Slack** to import a Slack theme. In Slack, go to **Preferences > Sidebar Theme** and open the custom theme option. From there, copy the theme color vector and then paste it into the **Input Slack Theme** input box in Mattermost. Any theme settings that are not customizable in Slack will default to the “Sapphire” standard theme settings.

Clock display
~~~~~~~~~~~~~

Choose a 12-hour or 24-hour time preference that appears on the time stamp for all posts.

Teammate name display
~~~~~~~~~~~~~~~~~~~~~

Configure how names are displayed in the user interface: nickname, username, or full name. The default for this setting is dependent on the `configuration set by the System Admin <https://docs.mattermost.com/configure/configuration-settings.html#teammate-name-display>`__.

Show online availability on profile images
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Online availability icons display on user profile avatars in the center channel by default. Disable this setting to hide online availability icons within the center channel.

Timezone
~~~~~~~~~

Select the timezone used for timestamps in the user interface and for email notifications.

.. note::
  
  In Mattermost v5.38 or earlier, timezone functionality `must first be enabled by the System Admin <https://docs.mattermost.com/configure/deprecated-configuration-settings.html#timezone>`__ by replacing ``false`` with ``true`` in ``config.json``. Timezone is enabled by default from Mattermost v6.0.

Website link previews
~~~~~~~~~~~~~~~~~~~~~

When available, the first web link in a message will show a preview of the website content below the message. This `setting must be enabled by your System Admin <https://docs.mattermost.com/configure/configuration-settings.html#enable-link-previews>`__.

Default appearance of image previews
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

When messages in Mattermost include images, an image preview can display directly below the message for image attachments, image link previews, and `in-line images <https://docs.mattermost.com/channels/format-messages.html#in-line-images>`__ over 100px in height. You can set this preference to **Expanded** or **Collapsed**.

.. tip::
  This setting can also be controlled using the slash commands ``/expand`` and ``/collapse``.

Message display
~~~~~~~~~~~~~~~

Select the formatting for messages in the center channel. **Compact** mode decreases the spacing around posts, collapses link previews, and hides thumbnails so only file names are shown. Some formatting types, such as block quotes and headings, are also reduced in size.

Collapsed Reply Threads
~~~~~~~~~~~~~~~~~~~~~~~

Collapsed Reply Threads offers an enhanced experience for users communicating in threads and replying to messages. Collapsed Reply Threads are generally available in Mattermost Cloud and from self-hosted Mattermost v7.0, and are enabled by default for all new Mattermost deployments. 

Depending on how your System Admin has enabled **Collapsed Reply Threads** for your workspace, it may already be enabled for you, or you may be able to enable this feature for your account. See our `organize conversations using Collapsed Reply Threads <https://docs.mattermost.com/channels/organize-conversations.html>`__ documentation to learn more about working with Collapsed Reply Threads.

Select to open threads
~~~~~~~~~~~~~~~~~~~~~~~

By default, selecting any part of a message opens the reply thread in the right hand sidebar. You can disable this behavior in **Settings > Display > Click to open threads**. When disabled, reply to a message or select the replies count to open the reply thread.

Channel display
~~~~~~~~~~~~~~~

Choose whether the text in the center channel is fixed width and centered, or full width.

Quick reactions to messages
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can react to messages quickly with your most recently-used emojis by hovering over a message.

Language
~~~~~~~~

Select which language Mattermost displays in the user interface. Options include:

- Deutsch - German
- English (U.S.)
- English Australian
- Español - Spanish
- Français - French
- Italiano - Italian
- Magyar - Hungarian
- Nederlands - Dutch
- Polski - Polish
- Português (Brasil) - Portuguese
- Română - Romanian
- Svenska - Swedish
- Türkçe - Turkish
- български - Bulgarian
- Pусский - Russian
- Yкраїнська - Ukrainian
- فارسی - Persian
- 한국어 - Korean
- 中文 (简体) - Simplified Chinese
- 中文 (繁體) - Traditional Chinese
- 日本語 - Japanese

Sidebar
-------

The channel sidebar includes `enhanced sidebar features <https://docs.mattermost.com/channels/customize-your-channel-sidebar.html>`__, including custom, collapsible channel categories, drag and drop, unread filtering, channel sorting options, and more.

The following sidebar settings apply to your current sidebar only:

**Group unread channels separately**

This feature groups unread channels at the top of the channel sidebar in an **Unreads** category. System Admins can `set the default of this setting <https://docs.mattermost.com/configure/configuration-settings.html#group-unread-channels-experimental>`__ for you.

Legacy sidebar settings
~~~~~~~~~~~~~~~~~~~~~~~

The legacy sidebar `must be enabled by your System Admin <https://docs.mattermost.com/configure/configuration-settings.html#enable-legacy-sidebar>`__. The following sidebar settings apply only to the legacy sidebar:

Channel grouping
^^^^^^^^^^^^^^^^

Channels can be grouped by type (public, private, or direct message), or all channel types can be grouped in a single list.

Channel sorting
^^^^^^^^^^^^^^^

Channels can be sorted within their channel sidebar sections alphabetically (default) or by most recent message.

Channel switcher
^^^^^^^^^^^^^^^^

Hide the channel switcher used to jump between channels quickly. The channel switcher can also be accessed using CTRL/CMD+K.

Autoclose direct messages
^^^^^^^^^^^^^^^^^^^^^^^^^

Hide direct message conversations that have been inactive for seven days. These conversations can be reopened using the **+** button in the channel sidebar, or by using the Channel Switcher (CTRL+K). This setting is experimental and `must be enabled by your System Admin <https://docs.mattermost.com/configure/deprecated-configuration-settings.html#autoclose-direct-messages-in-sidebar>`__.

Advanced
--------

Settings to configure when messages are sent.

Send messages on CTRL+ENTER
~~~~~~~~~~~~~~~~~~~~~~~~~~~

If **On for all messages** is enabled, pressing ENTER inserts a new line and pressing CTRL+ENTER posts a message. If **On only for code blacks starting with ```** is enabled, pressing ENTER inserts a new line inside an open code block and pressing CTRL+ENTER automatically closes the code block and posts the message. If disabled, pressing SHIFT+ENTER inserts a new line and pressing ENTER posts the message.

Enable post formatting
~~~~~~~~~~~~~~~~~~~~~~

This setting controls whether post formatting is rendered. When **On**, posts will be rendered with `Markdown formatting <https://docs.mattermost.com/channels/format-messages.html>`__, emoji, autolinked URLs, and line breaks. When **Off**, the raw text will be shown.

.. note::

  From Mattermost v7.0, this setting has been deprecated in favor of the `message formatting toolbar <https://docs.mattermost.com/channels/format-messages.html#use-the-messaging-formatting-toolbar>`__.

Enable join/leave messages
~~~~~~~~~~~~~~~~~~~~~~~~~~

This setting controls whether system messages about users joining or leaving a channel are visible. When **On** these messages will appear. When **Off**, these messages will be hidden. If any users are added to or removed from a channel, a system message will still be shown even if this setting is **Off**.

Preview pre-release features
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Turn on preview features to view them early, ahead of their official release.

**Show markdown preview option in message input box** Turning this on will show a **Preview** option when typing in the text input box. Select **Preview** to see what the Markdown formatting in the message looks like before the message is sent.

.. note::

  From Mattermost v7.0, this setting has been deprecated in favor of the `message formatting toolbar <https://docs.mattermost.com/channels/format-messages.html#use-the-messaging-formatting-toolbar>`__.

Performance Debugging
~~~~~~~~~~~~~~~~~~~~~

Turn on settings intended to help isolate performance issues while debugging. We don't recommend leaving these settings enabled for an extended period of time as they can negatively impact your user experience. Available only when `Enable Client Performance Debugging <https://docs.mattermost.com/configure/configuration-settings.html>`__ is enabled.

Deactivate account
~~~~~~~~~~~~~~~~~~

Use this setting to deactivate your account. After deactivating, an email notification is sent confirming the deactivation was successful.

Deactivating your account removes your ability to log in to the Mattermost server and disables all email and mobile notifications. To reactivate your account, contact your System Admin.

This is only available for accounts with email login, and if your System Admin has set ``EnableUserDeactivation`` to ``true`` in ``config.json``.

For accounts with other authentication methods such as AD/LDAP or SAML, or for accounts that do not have this setting available, contact your System Admin to deactivate your account.

Deprecated settings
-------------------

Notifications > Notification duration
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*Removed in June 16th, 2018 release*

In Mattermost v5.0 and later, desktop notifications will stay onscreen for five seconds when supported by the browser and operating system.

Display > Display font
~~~~~~~~~~~~~~~~~~~~~~

*Removed in July 16th, 2017 release*

Select what font is used.
