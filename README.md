# govCMS

This is the build for govCMS based on [Drupal 8](https://www.drupal.org/).

Please note this is a test build, and is most likely going to change, including structure, base profile, modules, themes, and other dependencies.

## Installation
**Dependencies**

- [git](http://git-scm.com)
- [composer](https://getcomposer.org)

To develop on or patch against govCMS, the source files should be downloaded and the project built.

1. Download repository from github
<pre><code>git clone --branch 8.x-3.x git@github.com:govCMS/govCMS.git</code></pre>

2. Enter the project root
<pre><code>cd govCMS</code></pre>

3. Run composer install to download dependencies
<pre><code>composer install</code></pre>

4. Run blt local setup [See more about BLT](https://github.com/acquia/blt)
<pre><code>blt local:setup</code></pre>
Note: You will need to ensure that the database 'drupal'(by default) exists and is empty. [See default.local.settings.php](https://github.com/govCMS/govCMS/blob/8.x-3.x/docroot/sites/default/settings/default.local.settings.php)(rename local.settings.php).

5. Enjoy a shiny govCMS build on Drupal 8 by visiting http://govcms.dev(by default), or using drush.
<pre><code>cd docroot</code></pre>
<pre><code>drush @self uli</pre>
