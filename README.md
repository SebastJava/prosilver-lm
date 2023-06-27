# Prosilver-lm: phpBB theme for LinuxMint

**WARNING: The contents you get here may not match what you see on the web site. Please [Check branches](https://github.com/SebastJava/prosilver-lm/branches) for the latest version.**

This Prosilver-lm is a custom tailored new look and feel for the LinuxMint forums. The LinuxMint forums are powered by [phpBB®](https://www.phpbb.com/) and this Prosilver-lm is a phpBB theme. This Prosilver-lm is what we call a "child" theme. It is based on the Prosilver parent theme. The Prosilver theme is the standard, default theme on phpBB. It is trustworthy. And this child theme here is just a small package. It only contains the modifications made on top of this standard and trustworthy Prosilver theme.

Don't get overwhelmed by the amount of files here. Most of these files are not part of the theme itself: preview, favicon, etc. You don't really need these. The files you need to look at are:

* template/ (directory)
* theme/ (directory)
* style.cfg

As you can see, there aren't many files in there. And that's all you need !

This Prosilver-lm being just a small child theme, this means it can easily and quickly be reviewed. And tested. And approved. And it won't be hard to merge the occasional updates coming from the parent theme. This child and parent theme structure is the most efficient and recommended way to work, as stated by phpBB. You can read all about phpBB theme creation on:

* https://www.phpbb.com/styles/installing/#a-editing (introduction)
* https://www.phpbb.com/styles/create/ (complete tutorial)

**See this Prosilver-lm for real ! Visit** https://sebastjava.com/forums/  

This is a forum showcase, powered by phpBB and featuring this Prosilver-lm. But that's only for a limited time. This website is just a temporary one and will probably be deleted on Jan 21, 2024.

But [What's Wrong With Minty ?](Whats-Wrong-With-Minty.md) Click to read all about it... And come back here to see how this Prosilver-lm is made better.

### Design improvements: colours and contrasts

> A contrast ratio of 3:1 is the minimum level recommended by [ISO-9241-3] and [ANSI-HFES-100-1988] for standard text and vision. The 4.5:1 ratio is used in this provision to account for the loss in contrast that results from moderately low visual acuity, congenital or acquired color deficiencies, or the loss of contrast sensitivity that typically accompanies aging.

source: https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html

All colors are not equal. I am using tools like:

* https://colorable.jxnblk.com/
* https://marijohannessen.github.io/color-contrast-checker/

These are used to evaluate the color contrasts with a foreground white text, for example. Or colored text on a white background. In those cases, I find it hard to get a nice green tint with a color contrast ratio of at least 3 or higher. It works much better with blue tones.

There can be some exceptions. The logo is not something that has to be read over a long period of time. It doesn't need to meet any contrasts standards. And I can always use some light green background tints with a dark foreground text, where applicable.

Anyway, those forums can hardly be made of only green tints on green tints. You need some contrasts. There is a need for neutral greys or blue tones. Here, the background body is made of a light and neutral grey. And all the forums posts are made of some very light background with dark grey foreground text. Thus, the contrast is always excellent. And the focus is naturally driven onto the inner posts, with their light backgrounds, as opposed to the outer grey body.

### Design improvements: page header and logo

* The "Lm" logo and "linuxmint forums" text are grouped together into one single SVG file. That's precision typography and alignments based on a variable weight [Exo 2 font](https://fonts.google.com/specimen/Exo+2?query=exo&vfonly=true). But don't worry, that text got converted to paths, so there is no need to download any font. No compatibility issues here.
* The site name and site description are not getting displayed anymore. So there is no redundancy with the logo, which already contains this nice and precise "linuxmint forums" typography.
* The logo and custom typography gets displayed on every devices, including on cellular phones, but with a reduced size for those, of course.
* Those two "headerbar" and "navbar", on top of every page, are now nicely grouped together. This makes it look less modular.
* This page header gets a linear color gradient with the same color values as found on LinuxMint's main website. For a coherent, consistent brand image.

### Design improvements: miscellaneous

* There are less colour gradients being used. It feels lighter, uncluttered, zen.
* The URL links got a bit darker, stronger.
* The posted pictures are all aligned to the middle, including the thumbnails. Before it felt unbalanced, as all the weight was on the left.

### Local tests (optional)

If you want to test this Prosilver-lm on your local computer before uploading it, you will need those:

* A local LAMPP or XAMPP installation. These are Apache distributions containing MariaDB, PHP, and Perl. It is a complete kit that will allow you to make a local phpBB installation. This way you can quickly test everything before uploading on your web server. Find all about this there: https://www.phpbb.com/support/docs/en/3.2/kb/article/installing-and-setting-up-your-own-web-server/
* A local and up-to-date phpBB installation. This Prosilver-lm was created on the latest stable phpBB release, version 3.3.10: https://www.phpbb.com/downloads/3.3/install

### Installation instructions (for LinuxMint administrators only!)

1. BACKUP everything. The most important is your entire database.
1. Update your phpBB forum software to the latest version: https://www.phpbb.com/downloads/3.3/update.
1. Make sure your `styles/prosilver` directory is unaltered. You should never modify this one, but create child themes instead. Else, just replace it with a fresh extract from the `phpBB-latest-version.zip`.
1. Download or clone this prosilver-lm directory from here on [SebastJava/prosilver-lm](https://github.com/SebastJava/prosilver-lm). (Click on that green "Code" button on top-right ↗)
1. Upload it onto your server at https://forums.linuxmint.com/styles/prosilver-lm/ (SFTP connection and administrator username and password required.)
1. Once the style is uploaded, navigate to the board's Administration Control Panel (ACP) to Customize -> Install Styles. You should see your recently uploaded styles listed (assuming you uploaded it to the correct location and the style is valid), with an option to "Install style". Simply click it and the installation is complete! [More info here](https://www.phpbb.com/styles/installing/).
1. In ACP > Customize > Styles section, you should deactivate the parent Prosilver theme. This way, this parent is still available for this Prosilver-lm to work, but the forum users cannot choose this Prosilver parent, so they won't end up with the phpBB logo replacing the LinuxMint logo...
1. You should also go to ACP > General > Board settings section, and check your Board style settings. There you can make this Prosilver-lm the default style and the guest style, among other things.

The official and complete installation instructions can be found [here on phpBB](https://www.phpbb.com/styles/installing/).

P.S.: Of course, you can start by keeping your current Minty theme as the default style and guest style, and just install this Prosilver-lm as another choice available for testing purposes.

### FlatUI Smilies update

1. The smilies could be updated too! The smilies are located at https://forums.linuxmint.com/images/smilies.
2. You could replace the default smilies with these new ones here: https://www.phpbb.com/customise/db/style/flatui_smilies/ Just follow the quick and easy instructions from there. Having trouble? The procedure is made even more simple now. You should be able to find my update topic about this procedure on https://www.phpbb.com/customise/db/style/flatui_smilies/support.

### Documentation and credits

Many information sources and tutorials helped into creating this Prosilver-lm:

* [phpBB](https://www.phpbb.com)
* [www.phpbb.com/styles/installing/](https://www.phpbb.com/styles/installing/)
* [www.phpbb.com/styles/create/](https://www.phpbb.com/styles/create/)
* [phpBB/support](https://www.phpbb.com/support/docs/en/3.3/kb/)
* https://www.phpbb.com/support/docs/en/3.2/kb/article/installing-and-setting-up-your-own-web-server/
* https://linuxhint.com/how-to-install-xampp-server-on-linux-mint-20/
* https://www.apachefriends.org/index.html
* [Xampp Panel Menu](https://cinnamon-spices.linuxmint.com/applets/view/146)
* [CSS Tutorial](https://www.w3schools.com/css/default.asp)
* [CSS Reference](https://www.w3schools.com/cssref/index.php)
* https://realfavicongenerator.net/
