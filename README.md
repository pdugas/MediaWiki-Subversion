MediaWiki-SVN
=============

MediaWiki Extension for Subversion Integration

MediaWiki-SVN currently a work-in-progress MediaWiki extension that adds
a `<svn/>` tag used to insert links to files in a Subversion repository.

### INSTALLATION

No configuration other than including the extension is required.  Add a line
like the one below to the bottom of your `LocalSettings.php` file.

> require_once("$IP/extensions/MediaWiki-SVN/SVN.php");

### USAGE

#### Directory Listing

Use the `<svn>URL</svn>` tag to insert a tabular list of directory entries in/under a given Subversion URL.  

> &lt;svn&gt;https://github.com/pdugas/MediaWiki-SVN/trunk&lt;/svn&gt;

or

> {{#svn:https://github.com/pdugas/MediaWiki-SVN/trunk}}

yield a table like this

![Screenshot showing directory listing](screenshot_01.png)

The links in the `Path` column lead to File Browser pages provided by this extension.  See below.

#### File Info

...

#### File Browser

...

### TODO LIST
* Add . and .. to the directory listing.
* Only publicly accessible repositories accessed via HTTP/HTTPS are currently supported.  Not sure if we want to change that due to potential security risks.

### AUTHORS
* Paul Dugas <paul@dugas.cc>
