.. _text-formatting:

===============
Text formatting
===============

Sometimes text should be formatted differently to designate a special meaning
or to make the text stand out. Usually this formatting is accomplished by
applying a different font treatment (bold, italics, or monospace).

.. note::

   *Monospace* is also called a *fixed-pitch* or *fixed-width*
   font. In monospace, each letter and character occupy the same amount of
   horizontal space. An example of a monospace font is Courier, and it
   looks as follows: ``monospace font``

Use the following general guidelines when formatting text:

-  To apply a font treatment, use the appropriate markup in your authoring
   tool. In RST, use a directive if one is available.
-  Don't apply font treatments to text in titles and headings.
-  Don't use capitalization to emphasize a term (for example, showing a
   general term in all capitals).
-  Don't use color alone to distinguish text.
-  Use quotation marks only as directed in this topic and in
   :ref:`quotation-marks`.

The following table shows the text formatting to use for different text
elements. The following style differences are highlighted:

- Content for Public Cloud versus Private Cloud
- Content that documents a CLI or API versus a GUI

.. list-table::
   :widths: 20 20 60
   :header-rows: 1

   * - Text element
     - Treatment
     - Output example
   * - API operation names
     - Regular text

       All lowercase
     - The following table describes the request attributes for the operation
       for migrating vaults.
   * - Application names
     - Regular text
     - You must configure the RabbitMQ application.
   * - Area (group box) names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the **Edit Signature** area, enter the text that you want to appear
       in your signature.
   * - Argument names
     - Monospace
     - To list or retrieve files from a node that's running the OpenCenter
       agent, use the ``file`` argument with the ``opencentercli`` node
       command.
   * - Attribute names
     - Monospace
     - The ``expires`` attribute denotes the time after which the token
       automatically becomes invalid.
   * - Box names
       (check box, combo box, group box, list box, spin box, text box, but not
       dialog box)
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select the **Manually configure server settings or additional server
       types** check box.

       Retype the password that you entered in the **Password** box.
   * - Button names
       (command, option, radio)
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select **Microsoft Exchange** and then click **Next**.
   * - Cascades
       (menu, field)
     - Bold

       Use **>** to separate.

       In RST, apply the ``:menuselection:`` directive.
     - Select **Start > Control Panel**, and then click the **Mail** icon.

       You can find more documentation about RackConnect in the **Community >
       Discussions > RackConnect** section of the MyRackspace Portal.
   * - Check box names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select the **Manually configure server settings or additional server
       types** check box.
   * - Code
     - Monospace

       In RST, apply the ``.. code-block:: console`` directive.
       For configuration files, use ``.. code-block:: ini``
       or ``.. code-block:: yaml`` as appropriate.
     
     - ``$ grep "ftp" /etc/xinetd.d/*``
       ``/etc/xinetd.d/vsftpd:service ftp``
       ``/etc/xinetd.d/vsftpd:server = /usr/sbin/vsftpd``

       To set the environment variable, run ``export token="token"``.
   * - Column names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - You can sort the backups by server by clicking the **Server** column
       label.
   * - Combo box names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select a name from the **Send to** list, or type a new name.
   * - Command names (CLI)
     - *(Public)* Monospace

       *(Private)* Bold, by applying the ``:command:`` directive in RST
     - *(Public)* You can check the architecture on Linux by using the ``uname
       -a`` command.

       *(Private)* You can check the architecture on Linux by using the **uname
       -a** command.
   * - Command syntax
     - Monospace
     - If a service isn't running, use the service command to start it, as
       follows:

       ``$ sudo service httpd start``
   * - Cross-references
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - Database names
     - *(GUI)* Bold

       *(CLI)* Monospace
     - *(GUI)* Start by creating a new database called **mytestdb**.

       *(CLI)* Start by creating a new database called ``mytestdb``.
   * - Dialog box names
     - Regular text
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.
   * - Directory names
     - *(Public, GUI)* Bold

       *(Private, CLI)* Monospace
     - *(Public, GUI)* Place all the contents of the uncompressed **wordpress**
       directory (excluding the directory itself) into the **/web/content/**
       directory, which is the root directory of the site.

       *(Private)* Place all the contents of the uncompressed ``wordpress``
       directory (excluding the directory itself) into the ``/web/content/``
       directory, which is the root directory of the site.

       *(CLI)* The following example shows a basic configuration for the FTP
       service, in a file in the ``/etc/xinetd.d directory``.
   * - Document titles
     - Italic

       **Note**: Use italic even if the title is a hyperlink.

     - For details about licensing for the NSX add-on component, see the
       "Licensing" section in the
       *Rackspace Private Cloud powered by VMware Customer Handbook*.
   * - Element names
     - Monospace
     - The ``message`` element returns a human-readable message that's
       appropriate for display to the end user.
   * - Email addresses
     - For examples, use bold.

       For actual email address, use the convention in your authoring
       environment to make the email address live.
     - **yourName@example.com**

       Contact the editor at kelly.holcomb@rackspace.com.
   * - Emphasis
     - Italic
     - Offset *must* be a multiple of the limit (or zero); otherwise, a Bad
       Request exception is generated.
   * - Environment variables
     - Monospace
     - You can set the ``MYSQL_HOST`` environment variable to the remote host's
       address.

       You can export the tenant ID to the ``$account`` environment variable
       and the authentication token to the ``$token`` environment variable.
   * - Error messages
     - Monospace
     - In SQL Server Management Studio, when you right-click a SQL Server 2012
       database and selecting **Properties**, the following error message
       appears:

       ``The user doesn't have permission to perform this action.``

   * - Examples, code
     - Monospace
     - ``$ grep "ftp" /etc/xinetd.d/*``
       ``/etc/xinetd.d/vsftpd:service ftp``
       ``/etc/xinetd.d/vsftpd:server = /usr/sbin/vsftpd``
   * - Field names, GUI
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the **Database Name** field, enter a database name identifier.
   * - File names and extensions
     - *(Public, GUI)* Bold

       *(Private, CLI)* Monospace
     - *(Public, GUI)* To remove the **vs\_quantum-api.cfg** file from the
       **haproxy.d** directory and retain it, you can move it to another
       directory.

       *(Private, CLI)* To remove the ``vs_quantum-api.cfg`` file from the
       ``haproxy.d`` directory and retain it, you can move it to another
       directory.
   * - Flags
     - Monospace
     - Use the ``-t`` flag to add a time stamp to the results.
   * - Folder names
     - *(GUI)* Bold

       *(CLI)* Monospace
     - *(GUI)* Copy the **index.php** file from your computer to the
       **content** folder.

       *(CLI)* Copy the ``index.php`` file from your computer to the
       ``content`` folder.
   * - Functions
     - Monospace
     - Container names are sorted based on a binary comparison, a single
       built-in collating sequence that compares string data using the
       ``memcmp()`` function, regardless of text encoding.
   * - Glossary terms
     - Italic, by applying the ``:term:`` directive in RST

       This directive also links the term to the definition in the glossary.
     - Rackspace provides an *IaaS* solution through a variety of complementary
       *services*.
   * - Group box names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the **Edit Signature** area, enter the text that you want to appear
       in your signature.
   * - GUI labels
     - Bold

       In RST, apply the ``:guilabel:`` directive.

       **Exception:** Show window, dialog box, wizard, page, panel, and screen
       names in regular text unless they need to be distinguished from the
       surrounding text. In such cases, use bold.
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.

       On the Choose Service page, select **Microsoft Exchange or compatible
       service**, and then click **Next**.

       Read the preliminary steps in the Configure Your Server wizard, and then
       click **Next**.
   * - HTML tags
     - Monospace
     - Avoid putting the ``xml:id`` attribute on the ``title`` tag.
   * - Hyperlinks (live)
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - Icon names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - To verify which OS version you're running, click the **Apple** icon in
       the top-left corner and then select **About This Mac**.
   * - Keyboard key combinations, names, and shortcuts
     - *(Public)* Bold

       *(Private)* Monospace
     - *(Public)* Press **Shift-G** and then press **Enter**.

       *(Private)* Press ``Shift-G`` and then press ``Enter``.
   * - Letters as letters
     - Italic
     - Place *i* before *e* except after *c*.
   * - Links (live)
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - List box names and selections
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - From the **Account Type** list, select **Exchange 2007**.

       To view these settings, select **Configure Backup** from the **Backup
       Actions** list.
   * - Menu names, commands, and sequences
     - Bold

       In RST, apply the ``:menuselection:`` directive to sequences.
     - Right-click the volume and select **Take Offline**.

       From the **Outlook** menu, select **Preferences**.

       Select **Start > Control Panel**, and then click the **Mail** icon.
   * - Messages (error, warning)
     - Monospace
     - In SQL Server Management Studio, when you right-click a SQL Server 2012
       database and selecting **Properties**, the following error message
       appears:

       ``The user doesn't have permission to perform this action.``

   * - Method names (HTTP)
     - Bold

       All capitals
     - Client authentication is provided through a REST interface by using the
       **GET** method.
   * - New terms
     - Italic
     - Cloud Servers that are built using the base Linux images are created
       without a dedicated swap partition and with *swappiness* (a measure of
       how the Linux kernel tries to use swap memory) set to 0.
   * - Option names, command
     - Monospace

       In RST, apply the ``:option:`` directive.
     - The ``--ip-addresses`` option specifies the IP address and an alias for
       the target.
   * - Option button names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select **Microsoft Exchange** and then click **Next**.
   * - Package names
     - Monospace
     - You must install the ``libvirt`` package.
   * - Page names
     - Regular text
     - On the Preferences page, you determine how frequently you receive email
       about all the activity on your account: daily, weekly, or both.

       On the Server Settings page, click **Check Name**, type your password,
       and then click **OK**.
   * - Panes, named and unnamed
     - Regular text
     - To verify that your SSL binding works, select your website in the
       Connections pane (if it's not already selected) and then click **Browse
       *ipAddress* (https)** in the Actions pane.

       In the navigation pane, select **Composing Email**.
   * - Parameter names
     - Monospace

       In RST, apply the ``:option:`` directive.
     - The ``display_description`` parameter is optional.

       Use the ``--flavor`` and ``--image`` parameters to specify the IDs or
       names of the flavor and image to use for the image.
   * - Paths
     - *(Public, GUI)* Bold

       *(Private, CLI)* Monospace
     - *(Public, GUI)* The path to Perl is **#!/usr/bin/perl -w**.

       *(Public, GUI)* In the URI path
       **https://incident.api.rackspacecloud.com/v1/...**, the API version is
       1.

       *(Private, CLI)* The path to Perl is ``#!/usr/bin/perl -w``.

       *(Private, CLI)* In the URI path
       ``https://incident.api.rackspacecloud.com/v1/...``, the API version is
       1.
   * - Permissions
     - Regular text
     - Log in to a shell as the user who has write permissions to
       ``/usr/local/bin`` on your local computer.
   * - Placeholder (variable) text
     - See :ref:`placeholder-variable-text`.
     - Not applicable
   * - Privileges
     - Regular text
     - The following examples assume that you're making the firewall changes
       as a normal user with sudo privileges.

       The user is granted ALL privileges on the database.
   * - Qualifiers
     - Italic
     - 1. *(Optional)* Enter a new name for the image.

       You can tell that the Managed Cloud post-build automation has
       successfully completed as follows:

       *(Windows servers)* The following file is created:
       **C:\\windows\\temp\\rs\_managed\_cloud\_automation\_complete.txt**

       *(Linux servers)* The following file is created:
       **/tmp/rs\_managed\_cloud\_automation\_complete**
   * - Quotations

       (content quoted from another source)
     - Quotation marks, or block quote formatting
     - "Scalability is key for our business," explained Nathan Goff, Inavero
       Operations Director and Partner. "There's nothing worse than making our
       clients look bad to their customers."
   * - Radio button names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select **Microsoft Exchange** and then click **Next**.
   * - Role names
     - Regular text
     - The full access role has the permissions to create, read, update, and
       delete resources within multiple designated products where access is
       granted.
   * - Sequences
       (menu, field)
     - Bold

       Use **>** to separate.

       In RST, apply the ``:menuselection:`` directive.
     - Select **Start > Control Panel**, and then click the **Mail** icon.

       You can find more documentation about RackConnect in the **Community >
       Discussions > RackConnect** section of the MyRackspace Portal.
   * - Syntax statements
     - Monospace
     - The main command used to change a file’s owner or group is ``chown``.
       The most common syntax used with ``chown`` is as follows:

       ``chown user:group file1 file2 file3``
   * - Tab names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the Microsoft Exchange dialog box, click the **Connection** tab and
       then select the **Connect to Microsoft Exchange using HTTP** check box.
   * - Terms, new
     - Italic
     - Cloud Servers that are built using the base Linux images are created
       without a dedicated swap partition and with *swappiness* (a measure of
       how the Linux kernel tries to use swap memory) set to 0.
   * - Terms, unique sense
     - Regular text

       Quotation marks on first use
     - The spelling checker "learns" the word. After it learns the word, the
       spelling checker ignores subsequent occurrences of the word in the
       document.
   * - UI labels
     - Bold

       In RST, apply the ``:guilabel:`` directive.

       **Exception:** Show window, dialog box, wizard, page, panel, and screen
       names in regular text unless they need to be distinguished from the
       surrounding text. In such cases, use bold.
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.

       On the Choose Service page, select **Microsoft Exchange or compatible
       service**, and then click **Next**.

       Read the preliminary steps in the Configure Your Server wizard, and then
       click **Next**.
   * - URLs (not live)
     - Bold
     - To access the web interface, open your web browser and navigate to
       **http://yourDomain.com/zipit-install.php**.
   * - URLs (live)
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - User input
     - *(GUI)* Bold

       *(CLI)* Monospace
     - *(GUI)* In the **Server** text box, type **outlook**.

       *(CLI)* Create a file by using a text editor, and insert the following
       code: ``<?php phpinfo(); ?>``

       *(CLI)* For the username, enter ``admin``.
   * - Variable (placeholder) text
     - See :ref:`placeholder-variable-text`.
     - Not applicable
   * - Variables, environment
     - Monospace
     - You can set the ``MYSQL_HOST`` environment variable to the remote host's
       address.

       You can export the tenant ID to the ``$account`` environment variable
       and the authentication token to the ``$token`` environment variable.
   * - Window names
     - Regular text
     - In the Network Connections window, right-click the private adapter and
       select **Properties**.
   * - Wizard names and wizard page names
     - Regular text
     - On the Welcome page of the Active Directory Domain Services Installation
       Wizard, ensure that the **Use advanced mode installation** check box is
       cleared, and then click **Next**.
   * - Words as words
     - Italic
     - Don't use *button* and *icon* interchangeably. If you're referring to
       a command button or toolbar button (labeled or unlabeled), use *button*.
       If you're referring to a graphic on a screen, window, or other area,
       use *icon*.
