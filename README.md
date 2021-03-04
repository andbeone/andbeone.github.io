# 1. andbeone-docs


## 1.1. [Installation](https://jekyllrb.com/docs/installation/)
Jekyll is a [Ruby Gem](https://jekyllrb.com/docs/ruby-101/#gems) that can be installed on most systems.

### 1.1.1. Requirements
- Ruby version 2.4.0 or higher, including all development headers (check your Ruby version using `ruby -v`)
- RubyGems (check your Gems version using `gem -v`)
- GCC and Make (check versions using `gcc -v`,`g++ -v`, and `make -v`)

### 1.1.2. Guides
For detailed install instructions, follow the guide for your operating system.
- [macOS](./MAC.md)
- [Ubuntu](https://jekyllrb.com/docs/installation/ubuntu/)
- [Other Linux](https://jekyllrb.com/docs/installation/other-linux/)
- [Windows](https://jekyllrb.com/docs/installation/windows/)


## 1.2. [Quickstart](https://jekyllrb.com/docs/)
Jekyll is a static site generator. It takes text written in your favorite markup language and uses layouts to create a static website. You can tweak the site’s look and feel, URLs, the data displayed on the page, and more.

Create a new Jekyll site at `./andbeone.github.io`.

    jekyll new andbeone.github.io
Change into your new directory.

    cd andbeone.github.io
Build the site and make it available on a local server.
    
    bundle exec jekyll serve
Browse to http://localhost:4000


## 1.3. Just the Docs: [Installation](https://github.com/pmarsceill/just-the-docs#installation)

Add this line to your Jekyll site's Gemfile:

```ruby
gem "just-the-docs"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: just-the-docs
```

And then execute:

    bundle install
Build the site and make it available on a local server.
    
    bundle exec jekyll serve
Browse to http://localhost:4000