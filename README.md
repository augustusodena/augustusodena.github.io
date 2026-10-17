# augustusodena.github.io

## Local preview

Use Ruby 3.1 or newer and Bundler. On Apple Silicon Macs, the scripts automatically
use Homebrew Ruby when available (`brew install ruby` if needed).

```sh
./script/setup
./script/serve
```

Open http://127.0.0.1:4000. Jekyll rebuilds after edits and LiveReload refreshes
the browser automatically. Stop the server with Ctrl-C. Rerun setup after changing
the Gemfile or lockfile.

- `index.html`: homepage biography
- `_layouts/`: shared page structure
- `css/main.css`: styles
- `assets/`: images and PDFs

To check a production build:

```sh
# Use the same Ruby as the scripts (Homebrew Ruby on Apple Silicon).
PATH="/opt/homebrew/opt/ruby/bin:$PATH" bundle exec jekyll build
```

Generated files and installed dependencies are ignored by Git. Commit source
changes and `Gemfile.lock`, then open a PR when ready.
