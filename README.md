# ![Flippy](https://github.com/backdrop-contrib/flippy/blob/1.x-1.x/images/flippy.png "Flippy for BackdropCMS")

Flippy is an ultra-simple module that generates previous/next pagers for content
types. On a content type's administration screen, you can turn Flippy on or off
for that content type. It will generate a unique pager for each content type,
so you can page through all of the Posts on the site, for example.

To change the position of the pager, visit the content type's Manage Display
page, where fields and other fieldish things can be dragged about. Flippy's
there, too.

If you turn on Flippy for a content type, but hide the pager in the Manage
Display page, its links will still be available in the theme layer when it comes
time to output `node.tpl.php`. If you like, you can weave the pager links right
into the node manually in your own templates. A block is also created so you
can add the block to your Layout wherever you wish.

## Installation

 - Install this module and its dependencies using the official 
  [Backdrop CMS instructions](https://backdropcms.org/guide/modules)

## Configuration and Usage

After installing and enabling the Flippy module:

- Go to **Structure > Content Types** (`/admin/structure/types`) and edit the 
content type on which you would like to have Flippy enabled.
- Check 'Build a pager for this content type' in the 'Flippy settings' tab. 
- You have options at this point:
  - Whether to add semantic previous and next links to the document HEAD.
  - Whether to show empty links. For example, if there is no "next" node, the 
  "next" label will be shown but without a link.
  - Input the label you want to display for the links. You can use tokens to 
  display elements of the current page being viewed.
  - Whether to display first/last links. It will ask you to input the labels if
  you check the checkbox.
  - Whether to loop through the nodes, in which case there won't be a first and 
  last node.
  - Whether to show the random link. (A label is needed if checked.)
  - Set up 'Truncate label length'. Long text will be truncated.
  - Set up 'Truncate ellipse' in case a label has to be shortened.
  - Sort by other fields.
    - If checked, choose the field for sorting the pager.
    - Select pager order.
  - Click the "Save Content Type" button to save the settings. 
  
You can control the placement of the Pager in the "Manage Display" section
for the content type in question. A block is also available in the Layouts 
section in case you want to position the Flippy pager that way (in this case,
you'll probably want to make the default pager hidden in the "Manage Display"
area to avoid having two pagers on the screen).

## Issues

Bugs and Feature requests should be reported in the 
[Issue Queue](https://github.com/backdrop-contrib/flippy/issues)

## Current Maintainers

 - [Laryn Kragt Bakker](https://github.com/laryn) - [CEDC.org](https://cedc.org)

## Credits

- Ported to Backdrop CMS by [Laryn Kragt Bakker](https://github.com/laryn) - [CEDC.org](https://cedc.org).
- Original author: [Jeff Eaton "eaton"](https://www.drupal.org/u/eaton)
- Current maintainer for the Drupal module: [Joshua Li "rli"](https://www.drupal.org/u/rli).

## License

This project is GPL v2 software. See the [LICENSE.txt](https://github.com/backdrop-contrib/flippy/blob/1.x-1.x/LICENSE.txt) 
file in this directory for complete text.
