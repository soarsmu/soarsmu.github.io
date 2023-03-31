# Development
Before making any change to the repo, please deploy the website locally and see whether changes will break the website.

If you haven't installed `jekyll`, do with

```gem install bundler jekyll```

Then go to the directory of this repo, and deploy by

```bundle exec jekyll serve```

More detailed instructions can be found <a href='https://jekyllrb.com'>here</a>.

## Notes for Apple Silicon Users
If you are using machines with Apple Silicon, please use the following commands:

```arch -arch x86_64 bundle exec jekyll serve```

## Docker users
Run `docker-compose up`.

For more info, refer to [Install Jekyll on your Mac with Docker Compose file 🤘 - Everything you need to get going](https://dev.to/stankukucka/install-jekyll-on-your-mac-with-docker-compose-file-everything-you-need-to-get-going-2alf)


# Allan Lab Website

This is the website of our academic research group at Leiden University.

This website is powered by Jekyll and some Bootstrap, Bootwatch. We tried to make it simple yet adaptable, so that it is easy for you to use it as a template. Please feel free to copy and modify for your own purposes.  You don't have to link to us or mention us (but of course we appreciate it).

Go to *aboutwebsite.md* to learn how to copy and modify this page for your purpose. 


Copyright Allan Lab. Code released under the MIT License.