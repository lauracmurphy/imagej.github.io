The ImageJ Documentation Wiki will no longer be available at location https://imagejdocu.tudor.lu, as the CRP Henri Tudor has merged to become the Luxembourg Institute of Science and Technology five years ago and the old domain will be discontinued. We want to take this as an opportunity to merge the resources on https://imagejdocu.tudor.lu with those here at https://imagej.net.

This guide covers the process of migrating a page from the ImageJ Documentation Wiki ([https://www.dokuwiki.org/dokuwiki DocuWiki]) to this ImageJ wiki ([https://www.mediawiki.org/wiki/MediaWiki MediaWiki]).

<ol>
<li>
<b>Create an ImageJ wiki account</b> if you do not already have one, by visiting the [[Special:CreateAccount]] page.
<li>
<b>Identify the ImageJ Documentation Wiki page you are migrating.</b> For this walkthrough, we'll choose the [https://imagejdocu.list.lu/plugin/analysis/colocalizationfinder/start Colocalization Finder] page.
</li>
<li>
<b>Grab the path to the page</b> by selecting it in the address bar and copying it to the clipboard. Here, this is <code>plugin/analysis/colocalizationfinder/start</code>.
</li>
<li>
<b>Grab the converted MediaWiki markup.</b> We have done a preliminary conversion of the wiki markup from DocuWiki format to MediaWiki format, and placed it online for you. Find your converted page at <code><nowiki>https://raw.githubusercontent.com/imagej/imagejdocu/master/[your-page].wiki</nowiki></code>, replacing <code>[your-page]</code> with the snippet from the previous step. For Colocalization Finder, the URL will be <code>https://raw.githubusercontent.com/imagej/imagejdocu/master/plugin/analysis/colocalizationfinder/start.wiki</code>. Copy the entire markup code to your clipboard.
</li>
<li>
<b>Navigate to the destination ImageJ wiki page.</b> On the ImageJ wiki, page names are capitalized with underscores. (Underscores become spaces in the page title.) For our migrated Colocalization Finder page, we'll use <code>https://imagej.net/Colocalization_Finder</code>. You should see a message like this:
<br>[[File:Creating-a-new-page.png|500px|link=]]
<br>Click "edit this page" to continue.
</li>
<li>
<b>Paste the converted wiki markup into the empty text area:</b>
<br>[[File:Add-wiki-markup.png|500px|link=]]
</li>
<li>
<b>Preview the results.</b> Scroll down below the text field, and click the "Show preview" button (in between "Save page" and "Show changes").
</li>
<li>
<b>Migrate needed images:</b>
<ol>
<li>Right-click and "Save Image As..." the images from your page on the ImageJ Documentation Wiki. For Colocalization Finder, there are two images: <code>cf_images.png</code> and <code>cf_table.png</code>.</li>
<li>In a separate browser tab, open the [[Special:Upload]] page and upload the images one by one. The Colocalization Finder images will become available from URLs <code>https://imagej.net/File:Cf_images.png</code> and <code>https://imagej.net/File:Cf_table.png</code>. Notice that MediaWiki always capitalizes the first letter of resources, including image files.</li>
<li>Back in our new Colocalization Finder page, we now replace the DocuWiki image link syntax with MediaWiki's syntax: e.g. <code><nowiki>{{:plugin:analysis:colocalizationfinder:cf_images.png?nolink&amp;400|}}</nowiki></code> becomes <code><nowiki>[[File:Cf_images.png|400px|link=]]</nowiki></code>. See MediaWiki's [https://www.mediawiki.org/wiki/Help:Images Help:Images] page for further details on formatting your images.</li>
</ol>
</li>
<li>
<b>Add categories to your page</b> so that it is classified correctly. The Colocalization Finder page is in the <code>plugins/analysis</code> subtree, so we will add <code><nowiki>[[Category:Analysis]]</nowiki></code> and <code><nowiki>[[Category:Plugins]]</nowiki></code>. These tags go at the very bottom of the wiki markup, each one on its own line. See [[Special:Categories]] for a complete list of available categories on imagej.net.
</li>
<li>
<b>Fix any remaining errors and imperfections.</b> Inspect the rendered page, noting any problems. Then scroll down below the page to find the text box containing the wiki markup code.
<ul>
<li>The <code>&lt;note warning&gt;...&lt;/note&gt;</code> block can become a <code><nowiki>{{Warning | ...}}</nowiki></code> block. (See documentation for [[Template:Warning]], [[Template:Notice]], [[Template:Tech]], [[Template:Box]], [[Template:Tip]], and [[:Category:Boxes|other boxes]].)</li>
<li>The red underlined words often highlight misspellings, and can be corrected now, since we have the opportunity.</li>
<li>See the [https://www.mediawiki.org/wiki/Help:Formatting MediaWiki formatting guide] for additional information on MediaWiki syntax.</li>
</ul>
</li>
<li>
<b>Click "Show preview" again</b>, as many times as needed, until everything looks good.
</li>
<li>
<b>Save the page when finished.</b> The "Save page" button locks in your new page!
</li>
</ol>