=== Archives by Category ===
Contributors:  Linda Cobb
Requires at least: 2.3.0
Stable tag: 2.3


== Description ==
This will create a list of all your posts.  They will be ordered alphabetically by category.  Category names will be anchor links so you 
can easily link to them.  You can put this as a list in your side bar or you can create an Archives page, whichever you prefer.

Version 1.0 works with WP prior to version 2.3
Version 2.2 prevents tags from showing up as a category in your list
Version 2.1 fixes errors when table prefix is not wp_

== Installation ==

1) Download, unzip, upload to your plugin directory and active the plugin.  Follow either set of directions below which ever works best for you.


ADD CODE TO A PAGE OR POST VERSION	

2) Create a new post or page.

3) Click the 'code' button in the edit window

4) Add the following line:
<!-- archivesbycategory -->

5) Save the file and post, You're done!  

OR USE THE HACK YOUR TEMPLATE VERSION OF THE DIRECTIONS	

2) Now an archive page is needed. You'll need to hack your template. Open up ‘archives.php’ [ not archive.php ] and find the line

<?php wp_list_categories(’title=0′); ?>

Yours might be slightly different. Remove that line and put in its place:

<?php echo archives_by_category(); ?>

3) Now all you have to do is create a page - call it ‘Archives’ and select ‘Archives’ as the page template. Nothing else needs to be done but to ‘publish’ the page.

I’ve built in anchor links to the page. It will get very long over time. You will want to create anchor links to each category. 
( See How and why you should use anchor links  http://herselfswebtools.com/2007/09/anchor-tags.html).

The archives page will update itself with all your news posts as you publish them. Nothing more need be done once this has been set up.

== Frequently Asked Questions ==

*If you are using Wordpress 2.3 download the ArchivesByCategory V 2.0 I totally cleaned up the MySQL and php and 
it is easier to read, for you to configure and should run a little faster.

*If you are using an earlier Wordpress version you need ArchivesByCategory V 1.0

If you need more information try here:
http://herselfswebtools.com/2007/10/here-is-a-quick-way-to-print-a-list-of-all-your-posts-by-category-in-wordpress.html

