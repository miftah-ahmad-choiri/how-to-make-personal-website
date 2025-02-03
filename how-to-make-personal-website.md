# How to make personal website on Github Pages

🚀 1. Update Fedora Packages
sudo dnf update -y

📦 2. Install Ruby and Development Tools
sudo dnf install -y ruby ruby-devel @development-tools redhat-rpm-config
sudo dnf install gcc-c++ make ruby-devel redhat-rpm-config

⚙️ 3. Configure Ruby Gems Path (Optional but Recommended)
echo '# Install Ruby Gems to ~/.gem' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/.gem"' >> ~/.bashrc
echo 'export PATH="$HOME/.gem/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

💎 4. Install Bundler and Jekyll via RubyGems
gem install bundler jekyll

✅ 5. Verify Installation
g++ --version
ruby -v
jekyll -v
jekyll 4.4.1

The easiest way to learn Jekyll is by following their simple tutorial. I just want to summarize the steps that I did to get up and running.

1. Opened a new VS Code project in a folder called `my-website/`. I had previously installed Ruby and RubyGems on my local laptop (running Windows 10), so I was able to go to the PowerShell terminal in VS Code and run:

   ```bash
   gem install jekyll bundler
   ```

   This installed Jekyll (somewhere in my `C:\Ruby31-x64` directory – sidenote, this is similar to the way I’m used to Conda installing Python packages). 

2. Then I ran:

   ```bash
   bundle init
   ```

   This created a blank `Gemfile` in the directory, and into that file, I added:

   ```ruby
   gem "jekyll"
   ```

3. After this, I ran:

   ```bash
   bundle
   ```

   This installed Jekyll because that’s what `bundle` does! It looks in your `Gemfile` and installs all the gems you need for the project.

4. At this point, I was able to create a toy file `index.html` in the `my-website/` root directory, and then run in the terminal:

   ```bash
   jekyll serve --livereload
   ```

   Jekyll is a static site generator! So when I run this command, it first automatically does a Jekyll build, which creates a new directory `_site/` containing all the pages to be published online as HTML.

5. With the `_site/` built, `jekyll serve` now gives me access to a local port at [http://localhost:4000/](http://localhost:4000/) that I can navigate to in a new internet browser window. The `--livereload` option ensures that most changes I make on VS Code are automatically shown in the browser! Some changes (like those to `_config.yml`) will need to have the server restarted to show them (i.e., a new Jekyll build has to run).
```

This markdown file includes the structure of the original content with clear sections for easier readability and navigation. Let me know if you'd like to modify it further!

```
------------------------
Edit Genfile
```bash
$ sudo dnf install npm
$ sudo npm install -g sass
$ gem install sassc
```

```bash
vi GemFile
```
```bash
source "https://rubygems.org"
gem "jekyll"
gem "github-pages", group: :jekyll_plugins
gem "jekyll-include-cache", group: :jekyll_plugins
```

