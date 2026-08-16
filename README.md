# corturn.github.io

Jekyll site published with GitHub Pages at <https://corturn.github.io>.
All page content is placeholder lorem ipsum; the styling is a neutral
placeholder too.

## Layout

```
_config.yml            Site title, nav menu, build settings
index.html             Home
about.md               /about/
tutoring.md            /tutoring/
contact.md             /contact/
blog.html              /blog/ — the post index, builds itself
_posts/                One .md file per blog post
_layouts/              default.html wraps every page; post.html wraps posts
_includes/             header.html and footer.html
assets/css/style.css   All styling. Variables at the top.
assets/images/         Artwork
```

## Publishing

```
git add -A
git commit -m "message"
git push
```

The live site updates a minute or so later. Build status is under the repo's
**Actions** tab on GitHub; a red X there means the site didn't rebuild.

## Adding a blog post

Create `_posts/YYYY-MM-DD-some-title.md`. The filename pattern is required.
Copy the front matter block from an existing post and edit it. The blog index
and the home page's recent-posts list both pick it up automatically.

A post dated in the future won't appear until that date.

## Local preview (optional)

Needs a newer Ruby than the one macOS ships. With Homebrew:

```
brew install ruby
echo 'export PATH="/opt/homebrew/opt/ruby/bin:$PATH"' >> ~/.zshrc
```

Then, in this folder:

```
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000. Pages rebuild as you save; `_config.yml` changes
need a restart.
