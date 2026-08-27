## Getting Started

* The Harvard Crimson Comp Website is a static site that is generated using Jekyll. It is deployed with GitHub Pages. To make modifications to the site, you will need `ruby` installed and the latest version of `gem`.

* Make sure that you've already `git clone`d this repo to your computer and are currently in the home directory of the repo.

* Once you've installed Ruby and ensured that you have the repo locally, add these two lines to the bottom of your `~/.bashrc` to ensure that every gem is stored in a local directory.
    ```
    export GEM_HOME=~/.gem
    export GEM_PATH=~/.gem
    ```

* Once you've done this, run the following commands:
    - `source ~/.bashrc` (enables the environment variables set above)
    - `gem install bundler` (install a gem that helps with package management)
    - `bundle install` (installs all the required gems)

* If any gem in particular gives you trouble during the `bundle install` process, you can try installing it directly with `gem install [gemname]`.

## Development
* In the home directory, run `bundle exec jekyll serve`. This will start a local development server.

* The default port is `4000` so visit `http://localhost:4000` to see the site!

* Any changes to CSS or HTML files will automatically trigger a rebuild, so no need to restart the server.

* If you update the information in `_config.yml` **or anything in `_data/`**, you _will_ need to restart the server. Livereload does not pick those up.

### If `bundle exec jekyll serve` fails with a missing-gem error

This project uses **Ruby 3.3.6 via rbenv** (see `.ruby-version`). macOS also ships
its own Ruby 2.6, and if that one is first on your `PATH` you get an error that
looks like a missing gem but isn't:

```
Could not find 'bundler' (2.3.5) required by your Gemfile.lock
```

Check which Ruby you're actually running:

```bash
ruby -v
```

If it says 2.6.x, rbenv's shims aren't ahead of the system Ruby. A common cause
is Anaconda — if your prompt starts with `(base)`, it has put itself first. Fix
it for the current shell with:

```bash
export PATH="$HOME/.rbenv/shims:$PATH"
```

`ruby -v` should now report 3.3.6 and the server will start. To make it stick,
put that line in your `~/.zshrc` **after** any Anaconda or other version-manager
setup, then open a new terminal.

## Deployment
* Since this website is hosted with GitHub Pages, you simply need to commit and push your changes to the `master` branch. This will automatically start a build process (note: this is only because GitHub Pages has automatic support for Jekyll).

* Wait about a minute and check <https://comp.thecrimson.com> to verify the site has been updated!