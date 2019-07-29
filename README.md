# hello-word
I hope I want something
# The syntax to use for patterns in the Rules file. Can be either `"glob"`
# (default) or `"legacy"`. The former will enable glob patterns, which behave
# like Ruby’s File.fnmatch. The latter will enable Nanoc 3.x-style patterns.
string_pattern_type: glob

 # A list of file extensions that Nanoc will consider to be textual rather than
# binary. If an item with an extension not in this list is found,  the file
# will be considered as binary.
text_extensions: [ 'coffee', 'css', 'erb', 'haml', 'handlebars', 'hb', 'htm', 'html', 'js', 'less', 'markdown', 'md', 'ms', 'mustache', 'php', 'rb', 'rdoc', 'sass', 'scss', 'slim', 'txt', 'xhtml', 'xml', 'json', 'asc' ]

 # The path to the directory where all generated files will be written to. This
# can be an absolute path starting with a slash, but it can also be path
# relative to the site directory.
output_dir: output

 # A list of index filenames, i.e. names of files that will be served by a web
# server when a directory is requested. Usually, index files are named
# “index.html”, but depending on the web server, this may be something else,
# such as “default.htm”. This list is used by Nanoc to generate pretty URLs.
index_filenames: [ 'index.html' ]

 # Whether or not to generate a diff of the compiled content when compiling a
# site. The diff will contain the differences between the compiled content
# before and after the last site compilation.
enable_output_diff: false

 prune:
  # Whether to automatically remove files not managed by Nanoc from the output
  # directory.
  auto_prune: true

   # Which files and directories you want to exclude from pruning. If you version
  # your output directory, you should probably exclude VCS directories such as
  # .git, .svn etc.
  exclude: [ '.git', '.hg', '.svn', 'CVS', 'assets' ]

 # The data sources where Nanoc loads its data from. This is an array of
# hashes; each array element represents a single data source. By default,
# there is only a single data source that reads data from the “content/” and
# “layout/” directories in the site directory.
data_sources:
  -
    # The type is the identifier of the data source.
    type: filesystem

     # The path where items should be mounted (comparable to mount points in
    # Unix-like systems). This is “/” by default, meaning that items will have
    # “/” prefixed to their identifiers. If the items root were “/en/”
    # instead, an item at content/about.html would have an identifier of
    # “/en/about/” instead of just “/about/”.
    items_root: /

     # The path where layouts should be mounted. The layouts root behaves the
    # same as the items root, but applies to layouts rather than items.
    layouts_root: /

     # The encoding to use for input files. If your input files are not in
    # UTF-8 (which they should be!), change this.
    encoding: utf-8

     # The kind of identifier to use for items and layouts. The default is
    # “full”, meaning that identifiers include file extensions. This can also
    # be “legacy”, primarily used by older Nanoc sites.
    identifier_type: full

 # Configuration for the “check” command, which run unit tests on the site.
checks:
  # Configuration for the “internal_links” checker, which checks whether all
  # internal links are valid.
  internal_links:
    # A list of patterns, specified as regular expressions, to exclude from the check.
    # If an internal link matches this pattern, the validity check will be skipped.
    # E.g.:
    #   exclude: ['^/server_status']
    exclude: []
ــــــــــــ🌟


{
  "description": "Gulp setup",
  "dependencies": {
    "gulp": "^3.9.0",
    "gulp-coffee": "^2.3.1",
    "gulp-concat": "^2.6.0",
    "gulp-connect": "^2.2.0",
    "gulp-if": "^2.0.0",
    "gulp-minify-css": "^1.2.1",
    "gulp-replace": "^0.5.4",
    "gulp-sass": "^2.0.4",
    "gulp-uglify": "^1.4.2",

     "js-yaml": "^3.4.3"
  },
  "scripts": {
    "gulp": "gulp"
  },
  "license": "MIT",
  "repository": {
    "type" : "git",
    "url" : "https://github.com/github/help-docs.git"
  }
}


