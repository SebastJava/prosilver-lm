# Prosilver-lm: a custom phpBB theme for the LinuxMint forums

Based on the parent, standard Prosilver theme from [phpBB®](https://www.phpbb.com/) Forum Software.  

### Installation instructions (for LinuxMint administrators only!)
1. Update your phpBB forum software to the latest version: https://www.phpbb.com/downloads/3.3/update.
2. Download this prosilver-lm directory from here on GitHub and extract it.
3. Upload it onto your server at https://forums.linuxmint.com/styles/prosilver-lm/ (SFTP connection and administrator username and password required.)
4. Once the style has been uploaded, navigate in the board's ACP to Customize -> Install Styles. You should see your recently uploaded styles listed (assuming you uploaded it to the correct location and the style is valid), with an option to "Install style". Simply click it and the installation is complete! [More info here](https://www.phpbb.com/styles/installing/).
5. In ACP > Customize > Styles section, you should deactivate the parent Prosilver theme. This way, this parent is still available for this Prosilver-lm to work, but the forum users cannot choose this Prosilver parent, so they won't end up with the phpBB logo replacing the LinuxMint logo...

NOTE: This Prosilver-lm is just a small child based on the Prosilver parent. You must first ensure you have a genuine, unmodified and up-to-date Prosilver parent theme before installing this Prosilver-lm. That's how it should always work anyway: creating child themes and leaving the parent unmodified.

### FlatUI Smilies update (for LinuxMint administrators only!)

1. The smilies should be updated too! The smilies are located at https://forums.linuxmint.com/images/smilies.
2. You could replace the default smilies with these new ones here: https://www.phpbb.com/customise/db/style/flatui_smilies/ Just follow the quick and easy instructions from there. Having trouble? The procedure is made even more simple now. You should be able to find my update topic about this procedure on https://www.phpbb.com/customise/db/style/flatui_smilies/support.

### Favicon update
The favicon is already created. Using the simple "Lm" version, without any background, makes it not so small for the classic 16x16 pixels size.  

Using https://realfavicongenerator.net/ a bunch of various files got created, for all browsers on all platforms. These files are contained in `favicon/favicon_package_v0.16.zip`.  

1. Extract this package in the root of your web site. If your site is `http://www.example.com`, you should be able to access a file named `http://www.example.com/favicon.ico`.
2. The `<head>` section is already edited in `template/overall_header.html`. No other action required.

