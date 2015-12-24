# automator

Do you find yourself having to convert .plist files to xml so you can edit them?  Do you create .mobileconfig files from .plist files using mcxtoprofile.py?  Do you download configuration profiles from your JSS and have to remove the signing and convert to xml?  Then these little automator contextual menus are for you!

These automator services that let you:

- **Convert to XML1** - Right-click on a .plist file, copy it to the desktop and convert it to xml1 (so you can edit it in a text editor)
- **Create MobileConfig** - Right-click on a xml1 .plist file and create a .mobileconfig from it (uses mcxtoprofile.py and assumes you've got the python script in your default path)
- **De-Sign MobileConfig** - Right-click on a .mobileconfig file downloaded from your JSS, remove the JSS signing and convert to xml1 (so you can edit it in a text editor)

**Downloading and installing**

You can download a zipped copy of the .workflow files here: https://github.com/amsysuk/automator/releases/download/0.2/services.zip.  Unzip and drop them into your ~/Library/Services folder to install.

**Usage**

Right click on the relevant .plist or .mobile config file and select the action from the services menu.  If you only have a couple of services they will be available directly in the contextual menu.

**Important Note 1** - You need to have a copy of mcxtoprofile (https://github.com/timsutton/mcxToProfile/blob/master/mcxToProfile.py) in your default path. Copy it to somewhere like /usr/local/bin/ to use the automator service.

**Important Note 2** - You can only use the mcxtoprofile service on an xml1 .plist file.  If its in binary format, use the xml1 convertor first.

**Important Note 3** - Add the .workflow files to ~/Library/Services so they appear in your contextual menu.

Thanks to the Mac Mule for the openssl code - https://macmule.com/2015/11/16/making-downloaded-jss-configuration-profiles-readable/

