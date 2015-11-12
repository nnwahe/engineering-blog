# Monsanto Engineering Blog

## Function

This is the engineering blog of Monsanto engineers, where we’ll share
ideas we have, open source software we use and have created. Watch
this space for future articles.

## New Posts

To contribute a new post, Monsanto engineers should fork the
`engineering-blog` repo, clone the fork, create a branch from develop,
create your new post in the `_posts` directory, check it in, push it,
create a [pull request][PR] from your new branch into develop on the
main version. After the PR is submitted it will go through the
approval process. Thanks

[PR]: https://github.com/MonsantoCo/engineering-blog/pulls (Monsanto Engineering Blog Pull Requests)

## Usage and development

*   Our engineering blog is built by [Jekyll][], so to work on it first
    install Jekyll. *If* you already have [Ruby][] and [RubyGems][]
    installed, this could be as easy as

        gem install jekyll --version '2.5.3'

    If you need to install those first, check out the
    [install documentation for Jekyll][jekyll-install].  You may also
    want to look at [rbenv][].

*   Fork the https://github.com/MonsantoCo/engineering-blog project
    using the Fork button in the top-right corner of its web page.

*   Next, checkout your fork of the site code

        git clone git@github.com:YOUR_USER/engineering-blog.git

    replacing `YOUR_USER` with your GitHub user name.

*   Change into the downloaded repository

        cd engineering-blog

*   **Create a new post**

    Copy one of the exsting posts, and make some changes.

        cp _posts/2015-01-22-stoop-our-first-open-source-release.md _posts/2015-04-01-this-is-a-new-post.md
        vi _posts/2015-04-01-this-is-a-new-post.md

    Again, be sure to update the 'frontmatter', that's the code
    between the `---` marks. Their functions are
    self-explanitory. After that build the site with Jekyll (see
    below) to see how it looks.

*   **Create a new page**

    If you're starting with html copy one of the exsting pages, for
    example `about.html` and make some changes

        cp about.html new_page.html
        vi new_page.html

    Be sure to update the 'frontmatter', that's the code between the
    `---` marks. Their functions are self-explanitory. After that
    build the site with Jekyll (see below) to see how it looks.

*   Build and server the site with Jekyll

        jekyll s

    Then you can view the site point your browser to
    http://localhost:4000/

*   Once you are done editing, add, commit and push the changes to GitHub

        git add .
        git commit -m "This is what I did to the code"
        git push

*   Finally, go to the web page for your repo and create a pull request
    into the develop branch of the MonsantoCo/engineering-blog.  Once
    submitted your PR will be reviewed and posted publicly.

[Jekyll]: http://jekyllrb.com/
[Ruby]: https://www.ruby-lang.org/ (Ruby Programming Language)
[RubyGems]: https://rubygems.org/ (Ruby Gems)
[jekyll-install]: http://jekyllrb.com/docs/installation/ (Jekyll Installation)
[rbenv]: https://github.com/sstephenson/rbenv (Ruby Environment)

## Push to production

You can just use the `update_prod.sh` script.

    bash update_prod.sh

You will get an email warning you about the CNAME setting for the site
that you can safely ignore.

Reload the site in a browser and enjoy!

## Questions?

Feel free to reach out on our
[Contact page](http://engineering.monsanto.com/contact/) or open an
[issue](https://github.com/MonsantoCo/engineering-blog/issues) for us
to fix. As always,
[pull requests](https://github.com/MonsantoCo/engineering-blog/pulls)
are welcome!


## License

Copyright (c) 2015, MonsantoCo
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.

* Neither the name of engineering-blog nor the names of its
  contributors may be used to endorse or promote products derived from
  this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

### Thanks
