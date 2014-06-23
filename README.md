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

##### Last updated 6/23/14
 * Fixed bug where it would throw an error on export; should be working in Sketch 3 now

##### Known issues:
 * Sketch bug: If you're trying to export an artboard and the object inside contains a border, the final exported size won't be correct. See [this issue](https://github.com/bomberstudios/sketch-framer/issues/31) for details. Easiest workaround is to manually create slices from your layer groups instead of generating slices from your artboards.
