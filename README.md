# Style Picker

https://main--style-picker--davidnuescheler.aem.page/media_1f4b7580caa1ffa601f975989772190931a0da0ba.mp4

Style Picker is a DA canvas extension for applying design-token styles to page
blocks, sections, and the page theme. It reads styles from the site's DA
spreadsheet and previews changes in the canvas.

## Installation

Replace `<org>` and `<site>` below with your DA organization and site names.

1. Create a spreadsheet at
   [https://da.live/sheet#/<org>/<site>/config/styles](https://da.live/sheet#/<org>/<site>/config/styles).
   The first column contains style names. Add columns for the style properties
   you want to manage, such as Background, Foreground, Accent color, Layout
   split, Horizontal alignment, Vertical alignment, and Font sizes. The picker
   reads this sheet as `/config/styles.json`.
2. Open the site's configuration at
   [https://da.live/config#/<org>/<site>/](https://da.live/config#/<org>/<site>/)
   open the `library` sheet, and add the following row:

   | title | path |
   | --- | --- |
   | Style Picker | `https://main--<site>--<org>.aem.page/tools/style-switcher/style-switcher.html` |

3. Save and publish the configuration. Open the site's page in DA canvas and
   select **Style Picker** from the extensions.

## Styled Banner

Use a **Styled Banner** block with one row containing an image cell and a
content cell, in either order. Add the **background** variant to the block or
section to place the image behind the content. A single image cell can also
contain text for the background variant. Style names can be added as block
variants or section styles; layout and font-size properties become data
attributes on the block. Without a style, the image banner uses a white
surface and dark text. The existing **Banner** block is unchanged.
