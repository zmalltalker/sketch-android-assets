# sketch-mobile-assets

_Based on [zmtalker/sketch-android-assets](https://github.com/zmalltalker/sketch-android-assets)_ 

This plugin for Bohemian Coding's Sketch app will generate iOS and Android assets for slices on your current page. Assets are automatically created at mdpi/hdpi/xhdpi/xxhdpi/xxxhdpi for Android and @1x/@2x for iOS, then named and organized according to platform conventions. 

**NOTE:** This plugin is designed for **Sketch 3**. It will overwrite any previously generated assets without prompting.

### Setup:
* Copy the `Generate Mobile Assets.jstalk` file and `/library` folder into your Sketch plugins folder 
 * _You can find your plugins folder by going to 'Plugins' > 'Reveal plugins folder'_
* Update `library/config.js` with your preferred naming conventions & DPI size

### To use:
* **Create & name slices for each of your assets**
* Run Plugins > Generate Android Assets, or hit &#8984;&#8679;A
* Choose a destination folder
* Magic!  

&nbsp;
- - -
&nbsp;  

##### Last updated 5/4/14
 * Updated to now work on Sketch v3.0.2
 * Weird empty slices shouldn't be generated anymore
 * Added file name + size config options
