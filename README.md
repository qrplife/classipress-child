# classipress-child
A simple child theme to customize a ClassiPress installation.

ClassiPress is a mature Wordpress application theme offered by [Appthemes](http://www.appthemes.com/themes/classipress/?aid=7039)

Using a child theme is the most reliable way to customize a Wordpress site based on ClassiPress (or any other WP theme I suppose). The problem with simply editing the theme directly is that when Appthemes releases updates any customizations you have made will be lost when you update your ClassiPress site.

This child theme is based on the sample that ships with ClassiPress and is used for two main purposes:

* Use CSS to alter how some default elements are rendered or to supress them altogether. These customizations are done in the style.css file. The current code supresses the location search box, hides the refine search widget, and hides the price display on listing shown by the `Classipress - Home Latest Listings`  widget and main page.
 
* Change some the text seen by site visitors to favor the term 'listing' instead of 'ad'. These customizations are done in `.po` and `.mo` files in the `/languages/` folder.

You're welcome to use this child theme as a starting point for your own ClassiPress customizations. For the languages I only support US English. I use the "translation" files to change some of the english text, not to translate into other languages.

* I recommend using Poedit to change/translate text from the `en_US.po` file and save as `.po` and `.mo`  or you can start with `classipress.pot` and save your custom `.po` and `.mo` files in the languages folder.

* The `functions.php`  from the ClassiPress child theme example has an additional function `child_theme_slug_setup()`  which loads the translation files from the child theme into ClassiPress.

