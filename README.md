# sketch-android-assets

Generate Android assets in Sketch.

## Installation

The basic procedure is the same regardless of which version of Sketch
you're running, and how you installed it; simply check out this
repository into your Sketch plugins directory and you're good to go.

The actual location of your Sketch plugins directory will vary,
however, depending on how you installed Sketch:

* For Sketch 2, use the `~/Library/Application Support/sketch/Plugins`
  folder.
* If you bought Sketch 3 from the App Store, use the
  `~/Library/Containers/com.bohemiancoding.sketch3/Data/Library/Application Support/sketch/Plugins`
  directory
* If you downloaded Sketch 3 from the Bohemian Coding site, use the
  `~/Library/Application Support/com.bohemiancoding.sketch3/Plugins`
  directory

Once you have checked out the plugin repository into the relevant
directory, you'll find the plugin functions under the Plugins menu in Sketch.

## Base resolution (experimental)

If the default assumption of one pixel in your Sketch designs being
equal to 1dp, you can use a different factor either for a single
Sketch document or for all documents you create.

To use another resolution as the base, add a file named
`.android_assets` (note the period at the beginning of the file name)
with the contents

```
base_density:xxx
```

where `xxx` is the density you want to use, any of:

* mdpi
* hdpi
* xhdpi
* xxhdpi
* xxxhdpi

So if 1 pixel in your design should be 1 pixel on an MDPI display, use
`base_density:mdpi`.

If you don't specify a base density, the plugin will ask you which one
to use for the document you're currently working on and create a
configuration file for that. This means that the next time you run the
plugin for this document, the density you selected previously will be used.

The file should be placed in one of two places:

* if you're setting up defaults for a single Sketch document, add the
  file to the same directory as your Sketch document
* if you're setting up a default for *all* your Sketch document, add
  it to your home folder (`/Users/<yourusername>/`).

To use `hdpi` as your default density for all your Sketch documents,
simply enter this command into a Terminal window:

```shell
echo "base_density:hdpi" > ~/.android_assets
```
