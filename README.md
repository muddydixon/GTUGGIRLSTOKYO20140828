Web Server
------
```
python -m http.server 5000
python -m SimpleHTTPServer 5000
plackup -MPlack::App::Directory -e 'Plack::App::Directory->new(root => ".")->to_app'
ruby -run -e httpd -- --port=5000 .
ruby -rwebrick -e 'WEBrick::HTTPServer.new(:Port => 5000, :DocumentRoot => ".").start'
```
