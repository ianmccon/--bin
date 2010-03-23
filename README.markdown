MarkBin Script Collection
========================

What is this?
-------------

This is just a collection of small useful scripts that make working with the command line easier for me.

To make the most of these scripts, install them on every new computer that you work on. They will help to get you up and running with all your defaults in place.

Installation
------------
Ensure that ~/bin is part of your path and
run <pre><code>git checkout git://github.com/markmcconachie/--bin.git ~/bin </code></pre>

Updating
--------
To update the scripts
run <pre><code>update-markbin</code></pre>

Uninstall
---------
Just remove the ~/bin directory

How do I use this?
------------------

### Git

Edit settings in ~/bin/config-git to reflect your desired git settings and run
<pre><code>config-git</code></pre>

### SSH Keys

Run 
<pre><code>gen-key</code></pre>

This will generate an rsa key on your local machine. Enter a passphrase for added security.

<pre><code>run install-key [hostname]</code></pre>

Enter your password for the remote machine. This will copy the key to the remote machine and deal with permissions etc.

Now when you run

<pre><code>ssh [hostname]</code></pre>

you will be logged straight in. (If you chose to add a passphrase you will need to enter it or have your operating system remember it.)

#### Getting your key (for adding to github etc)
<pre><code>get-public-key</code></pre>