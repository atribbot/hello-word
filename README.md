# hello-word
I hope I want something

<!DOCTYPE HTML>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>A Brand New nanoc Site - <%= @item[:title] %></title>

     <!-- you don't need to keep this, but it's cool for stats! -->
    <meta name="generator" content="nanoc <%= Nanoc::VERSION %>">
  </head>
  <body>
    <div id="main">
      <%= yield %>
    </div>
    <div id="sidebar">
      <h2>Documentation</h2>
      <ul>
        <li><a href="http://nanoc.ws/docs/">Documentation</a></li>
        <li><a href="http://nanoc.ws/docs/tutorial/">Getting Started</a></li>
      </ul>
      <h2>Community</h2>
      <ul>
        <li><a href="http://groups.google.com/group/nanoc/">Discussion Group</a></li>
        <li><a href="irc://chat.freenode.net/#nanoc">IRC Channel</a></li>
        <li><a href="http://github.com/nanoc/nanoc/wiki/">Wiki</a></li>
      </ul>
    </div>
  </body>
</html>
