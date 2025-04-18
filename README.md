# Mobile Sensing Technology

This website showcases the embedded system development delivered to the Hannigan Lab
at CU Boulder, in support of various research efforts which require in-situ collection
of air pollution sensor data.

The original website was decommissioned around mid-2019.

The static content here is a reproduction of the archived site from the WaybackMachine project. [Ref](https://web.archive.org/web/20190317111610/http://mobilesensingtechnology.com/).

## Reproduction

[This utility](https://github.com/ShiftaDeband/wayback-machine-downloader) was used to do an initial scrape and stitching of the assets from the WaybackMachine archive.org hosted site.
Note that this is a fork of an original `wayback-machine-downloader`, which has recent updates to fix issues with the original unmaintained project.

The scraped assets were not host-ready. The following steps were carried out manually.

1. `wp-content` and `wp-includes` directories were removed from the exclude directives in the `robot.txt` file
2. all `index.html` files were updated to remove the `http://mobilesensingtechnology.com` prefix (leaving a root reference `/`) in instances of `src=` and `href=` 
3. all `.js` and `.cs` files in `wp-includes` and `wp-content` were updated to remove `?ver=*` suffixes
4. all instances of `?ver=...` (i.e. regex `\?ver=.*?\'`) were removed from `index.html` files (thus establishing a link to the modified files from step 3., without the browser query-param confusion)

## Hosting

The static content in this repo is hosted with GitHub Pages.