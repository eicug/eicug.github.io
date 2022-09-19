# eicug.org

Starting the development server to open the pages on local network:

```bash
bundle exec jekyll serve --trace --host 0.0.0.0
```

For Ruby versions ~> 3.0 you may need to add an explicit dependency on `webrick` to the `Gemfile`:

```
gem 'webrick', '~> 1.7'
```

Server side:
```bash
cd t
wget --convert-links -r https://eicug.github.io/
cd ..
rm -fr public_html
mv t/eicug.github.io/ public_html
```
