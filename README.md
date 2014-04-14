# sketch-mobile-assets

Based on https://github.com/zmalltalker/sketch-android-assets. This plugin for Bohemian Coding's Sketch app will generate iOS and Android assets for slices on your current artboard. 


## Notes:
  * This was designed for Sketch 2 - Sketch 3 now lets you do nearly all of this from within the app
  * This plugin assumes you're designing @1x 
  * Android naming convention: `android/drawable-{DPI}/ic_{prefix}_{slice name}_{suffix}_{width}.png` _(i.e. `ic_btn_menu_pressed_24.png`)_
  * iOS naming convention: `iOS/ic_{prefix}_{slice name}_{suffix}_{width}{_@2x}.png` _(i.e. `ic_btn_menu_pressed_24@2x.png`)_
  * This will overwrite any previously generated assets without prompting


## To use:
  * Copy the 'Generate Mobile Assets.jstalk' file to `~/Library/Application Support/sketch/Plugins` 
  * Name your artboards (this will become the `{suffix}`- i.e. normal, pressed, disabled, etc)
  * Create & name slices for your assets (this will become `{slice_name}`)
  * Run Plugins > Generate Android Assets
  * Choose a destination folder + enter a prefix 
  * Magic!


## Known issues:
  * Occasionally, this winds up generating some weird empty layers at the top of your artboards. If these appear, hit undo and they'll be removed.
