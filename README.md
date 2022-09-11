ReShade API Examples
====================

Detailed API documentation can be found at https://crosire.github.io/reshade-docs/index.html.

## [04-texture_dump](/examples/04-texture_dump)

Dumps all textures used by the application to image files on disk (into `[executable name]_0x[CRC-32 hash].bmp` files).

## [05-texture_replace](/examples/05-texture_replace)

Replaces textures before they are used by the application with image files from disk (looks for a matching `[executable name]_0x[CRC-32 hash].bmp` file and will then load it annd overwrite the image data from the application before texture creation).\
One can use the [texture_dump](#04-texture_dump) add-on to dump all textures, then modify some and use [texture_replace](#05-texture_replace) to inject those modifications back into the application.

