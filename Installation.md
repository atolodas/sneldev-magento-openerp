# Introduction #

This page describes the installation of the Magento-OpenERP interface.

_Our interface was tested with the following versions :
  * Magento Server 1.3 to 1.6.
  * OpenERP Server 6.0 running under Linux._


The PDF version of the Installation Guide can be found here :
[Installation Guide with screenshots](http://code.google.com/p/sneldev-magento-openerp/downloads/detail?name=Installation%20Guide.pdf&can=2&q=)

# 1. Magento #

If you do not have Magento installed yet, please follow the instruction from Magento web site to install it:

http://www.magentocommerce.com/knowledge-base/entry/magento-installation-guide


## 1.1. Magento extension installation ##

There are two options to install the Magento extension. You need to follow only one of them:

### Via Magento Connect ###

  1. Go to Magento Connect and get the extension key for our extension.
  1. In the Admin Panel of Magento, go to System / Magento Connect / Magento Connect Manager
  1. Copy the extension key and click on Install


### Via Google Code ###

  1. Download the latest version of the Magento extension in the download section of this project.
  1. Extract it in your Magento root folder. Make sure to keep the directory structure from the compressed file.


## 1.2. Magento Extension configuration ##

### 1.2.1 Refresh the extension cache ###

  1. In the Admin Panel, go to System / Cache Management.
  1. Select Configuration and Web Services Configuration.
  1. In the Actions menu select Refresh, and then click on Submit button.


### 1.2.2 Create a Web Services User ###

  1. In the Admin Panel, go to System / Web Services / Roles.
  1. Add a new role, any name is fine.
  1. Under Roles Resource tab, select All for Resource Access menu.
  1. Save Role.
  1. In the Admin Panel, go to System / Web Services / Users.
  1. Add a new user; make sure the user is active. Please remember the User Name and API Key, you will need them to configure OpenERP.
  1. In User Role tab, select the role you created earlier.
  1. Save User.


# 2. OpenERP #

You will also need a working OpenERP server and at least one client.
Follow the following link for instruction to install OpenERP server and client :

http://doc.openerp.com/install/index.html


## 2.1. OpenERP Module ##

  1. If you do not have a OpenERP database yet, create one.
  1. Download the latest version of the OpenERP module on our download page.
  1. Connect to you database and go to Administration / Modules Managments / Import module
  1. Select the downloaded .zip file and import.
  1. Select the sneldev\_magento module.
  1. Click on Schedule for Installation then Apply Scheduled Upgrades

If the module is installed correctly, you should see a new Magento tab in the OpenERP menu.


## 2.2. Automatic Synchronization script _(optional)_ ##

This step is only needed if you need the automatic synchronization. You can come back to this step later.

  1. Download the latest version of the script on our download page.
  1. Extract the file anywhere on the machine running the OpenERP server.
  1. Make sure the OpenERP server has read access to the file.
  1. Open the file in your text editor and configure the settings of your OpenERP server and database.


# 3. Start using the connector #

See our [QuickStartTutorial](QuickStartTutorial.md) page for help.

# Need help ? #

You need professional help with the installation or you are interested with our pre-installed solutions ?

Don't hesitate to contact us here : http://www.sneldev.com/en/contact.html