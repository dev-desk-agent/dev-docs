# Developer Training Documentation

This repository contains documentation for developer trainings focused on improving the development process.

## How to Use

This documentation is published using GitHub Pages. You can access it at the published URL.

## Local Development

To run this site locally:

### Prerequisites

#### macOS

```bash
# Install Homebrew if not installed
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Ruby
brew install ruby

# Add Ruby to your PATH
echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc

# Install Jekyll and Bundler
gem install jekyll bundler
```

#### Windows

1. Download and install Ruby+Devkit from [RubyInstaller](https://rubyinstaller.org/downloads/)
2. During installation, check the option to run `ridk install`
3. Choose option 3 when prompted by the MSYS2 installer
4. Open a new command prompt and run:

```bash
gem install jekyll bundler
```

#### Linux (Ubuntu/Debian)

```bash
# Update package lists
sudo apt-get update

# Install Ruby and dependencies
sudo apt-get install ruby-full build-essential zlib1g-dev

# Update gem system
sudo gem update --system

# Configure gem installation path
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

# Install Jekyll and Bundler
gem install jekyll bundler
```

### Running the site

1. Clone this repository
2. Run `bundle install`
3. Run `bundle exec jekyll serve`
4. Open `http://localhost:4000` in your browser
