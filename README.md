# sketch-android-assets

Generate Android assets in Sketch.

**This plugin is no longer maintained, and probably not required
either**. Sketch has received native support for exporting assets for
Android. To use this, use Sketch's native export settings, with a few
tweaks:

* First click the settings dialog in the Export section, and select
  "Edit presets"
* In the dialog that appears, select the "Android" item in the list,
  and prepend `drawable-` to each "Prefix/suffix" text box in the
  list. So rather than having `mdpi/` in the `1x` item, enter
  `drawable-mdpi/`

Now, when exporting simply select the "Android" preset and click the
Export button

If for some reason you still want to use this plugin, use Git to
checkout a previous version.
