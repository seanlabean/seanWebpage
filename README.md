# Sean's Webpage

Built off of the al-folio template: originally, **al-folio** was based on the [\*folio theme](https://github.com/bogoli/-folio) (published by [Lia Bogoev](http://liabogoev.com) and under the MIT license).

## Purpose

As a challenge to myself, I wanted to create and maintain my personal webspace provided by Drexel University: [Sean's Page](https://physics.drexel.edu/~slewis/). The hope is to use this as a professional blog/self-advertisement.

## Other

Currently a work in progress...

## Compiling and Publishing

On my machine, after making edits to website dependencies I need to compile using the blog-aware site generator jekyll (written in ruby): `bundle exec jekyll build`
Then, send the compiled site to the hosting server, in this case: Drexel University Physics Department's server. `scp -r {my_local_website_dir}/_site/* {cluster_username}@{cluster_url}:~{cluster_username}/public_html`