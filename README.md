# KiCad documentation images

New Kicad documentation repository.

This is a simple collection of the images from the KiCad help documents
at https://code.launchpad.net/~kicad-developers/kicad/doc

The images in each ODT file have been extracted into folders in the
following format:

> <language>/<component>/images

Common images, such as icons and the kicad logo are broken out into
the "common" directory, so that they can be reused among all languages,
and changing one can change all of them.

Things common to a particular componet (e.g. non-localised GUI
elements or non-localised diagrams) can be put in:

> <common>/<component>/images

Again, this makes sharing amongst languages easy.

## Issues

For now, the LibreOffice image "names" have been kept, as choosing
good filenames probalby can't be automated, and it means you can then
used "find" for a "missing" image if you can't see it.

Icons also have massive amounts of duplication and obsolescence. Probably
a good number of the icon files can be just replaced with raw icons from
the KiCad codebase, and duplicates can just be killed off. For now, they
are just all dumped in common/icons.