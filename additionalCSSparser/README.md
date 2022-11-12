# additionalCSSparser

### the popular content management system Wordpress allows developers to add custom css to a file under the customization tab called "additional CSS". While this functionality is undoubtedly useful, for sites that have been around the sun a few times (especially those that have had multiple cooks in the kitchen), this file can become a bit of a nightmare.

Lets face it, a lot of developers don't put very much effort into writing documentation and some don't write any. If you assume management responsibilities for a Wordpress site that has 600 lines of "additional css", ambiguous variable names, and no comments; you're up shits creek without a paddle. You can't just go in there and start removing code, who knows what will break if you remove "JBsHeaderClass" on line 324.

However, it should not be difficult to create a simple Python program to resolve this confusing dillemma, and provide developers with a simple means of analyzing all of the custom CSS that's in use on a wordpress site

1. with input of a sitemap.xml URL, iterate through each page of a website, use beautiful soup to fetch source code and save everything locally.


python import: JSON, BeautifulSoup4                                                                                                              


                               
2. iterate through local copies of pages, appending new information to a working key-value store (dictionary) of the additional CSS classes the site is currently using, how many pages use each style, and which pages those are.

... the rest should be self explanatory.
