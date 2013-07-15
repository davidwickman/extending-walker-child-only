# Understanding the Walker Class

This is a repo of code I edited from Understanding the Walker Class | Wptuts+ http://goo.gl/m3iTY to work with my current version of Wordpress

Originally written by Stephen Harris on May 14th 2012 for Tutsplus.com

## Extending the Walker

First of all we don’t want to display top-level parents. Recall that the function responsible for the opening `<li>` tag and the link is `start_el` and the function responsible for the closing `</li>` tag is `end_el`. We simply check if we are at the parent level. If we are, we don’t do anything. Otherwise, we continue ‘as normal’ and call the function from the `Walker_Nav_Menu` class.