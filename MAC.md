# 1. [Jekyll on macOS](https://jekyllrb.com/docs/installation/macos/)


## 1.1. Install Command Line Tools
To install the command line tools to compile native extensions, open a terminal and run:

    xcode-select --install

## 1.2. Install Ruby
Jekyll requires **Ruby v2.4.0** or higher. macOS Catalina 10.15 ships with Ruby 2.6.3. Check your Ruby version using `ruby -v`.

If you’re running a previous version of macOS, you’ll have to install a newer version of Ruby.

### 1.2.1. With Homebrew
To run the latest Ruby version you need to install it through [Homebrew](https://brew.sh/).

    # Install Homebrew
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

    # Install Ruby
    brew install ruby

Add the brew ruby path to your shell configuration:

    # If you're using Zsh
    echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc

    # If you're using Bash
    echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.bash_profile

    # Unsure which shell you are using? Type
    echo $SHELL

Relaunch your terminal and check your Ruby setup:

    which ruby
    # /usr/local/opt/ruby/bin/ruby

    ruby -v
    ruby 2.7.2p137 (2020-10-01 revision 5445e04352)

You’re now running the current stable version of Ruby!

## 1.3. Install Jekyll
After installing Ruby, install Jekyll and Bundler.

### 1.3.1. Local Install
Install the bundler and jekyll gems:

    gem install --user-install bundler jekyll

Get your Ruby version:

    ruby -v
    ruby 2.7.2p137 (2020-10-01 revision 5445e04352)

Append your path file with the following, replacing the `X.X` with the first two digits of your Ruby version:

    # If you're using Zsh
    echo 'export PATH="$HOME/.gem/ruby/X.X.0/bin:$PATH"' >> ~/.zshrc

    # If you're using Bash
    echo 'export PATH="$HOME/.gem/ruby/X.X.0/bin:$PATH"' >> ~/.bash_profile

    # Unsure which shell you are using? Type
    echo $SHELL

Check that `GEM PATHS:` points to your home directory:

    gem env

### 1.3.2. Global Install

#### 1.3.2.1. On Mojave (10.14)
Because of SIP Protections in Mojave, run:

    sudo gem install bundler
    sudo gem install -n /usr/local/bin/ jekyll

#### 1.3.2.2. Before Mojave (<10.14), run:

    sudo gem install bundler jekyll
