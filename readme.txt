=== Easy Post-to-Post Links ===
Tags: post, links, shortcut
Contributors: coffee2code
Version: 0.9

Easily reference another post in your blog using a shortcut, either by id or post slug.  The shortcut is replaced with the hyperlinked title of the referenced post.

== Installation ==

1. Upload to your plugins folder, usually `wp-content/plugins/`
2. Optional: Change configuration options in the file to your liking 
3. Activate the plugin on the plugin screen
4. Use one of the two forms of the shortcut to reference another post when the need arises.

== Frequently Asked Questions ==

= How do I use the shortcut in a post to link to another post? =
To easily link to another post, in your post:
a. type <!--post="22"--> (where '22' is the post id of the post you want to reference)
-or-
b. type <!--post="hello-world"--> (where "hello-world" is the post slug of the post you want to reference)

In either case, if a matching post is found, the shortcut will be replaced with the title of the post hyperlinked to
the post's permalink.

= Where do I find the ID for the post I want to reference? =

Some of the ways:
* In the admin section, under "Manage", it should be the first column in the posts listing.
* If you aren't using rewrite rules, it is the number after the "p=" in the post's URL.

= Where do I find the post slug for the post I want to references? =

Some of the ways:
* If you know the manner in which post titles are turned into slugs (i.e. make all characters lowercase, turn spaces
into underscores, and remove all other alphanumeric characters). you could figure it out on your own, i.e.
"Hello World!" becomes "hello-world"
* If you are using rewrite rules, it is the part that follows the date in the URL.
* If you edit the post, it'll appear under the "Advanced" section

= What happens if it doesn't find a post that matches what I put within the double-quotes? =

The shortcut will be replaced with an empty string (i.e. nothing).

= Are there any special situations where this might not work properly? =

An incorrect substitution will take place if you happen to have a post with a numerical title (and thus a numerical post slug).
