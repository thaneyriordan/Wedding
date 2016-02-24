Kay + Dave's Wedding Website
=============================
This is the wedding website of [Kaitlin Thaney](http://twitter.com/kaythaney) and [David Riordan](http://twitter.com/riordan). Yes, we're total nerds obsessed with open source and open licensing.

# Getting started with editing
* Clone the directory to your local computer
 * `git clone git@github.com:thaneyriordan/wedding.git`
* Install the requisite code
 * `bundle install`
  * if this fails, you're going to want to install Bundler for Ruby
   * `sudo gem install bundler`

# Content Updates
* Homepage text updates at `index.html`
* Image assets live in `/images`
 * Check the CSS + the page layouts for where they are
* Icons from [Font Awesome](https://fortawesome.github.io/Font-Awesome/) can be changed with their `fa-` codes
 * located in both the HTML + the CSS files

Any problems getting things figured out, file a new [Issue](https://github.com/thaneyriordan/wedding/issues).


# Using Vagrant for server
* Get to wedding website directory from Terminal
* type `vagrant up` into the Terminal to start server
* type `atom .` into the terminal to start your code editor
* Go to [http://127.0.0.1:4000](http://127.0.0.1:4000) to visit website
* Changes will update locally as you save the files
* When you're done working on the website, type `vagrant suspend` to stop the virtual machine


# Pushing to live website
When you have completed a package of changes you'd like to push to the live website:
* make sure you're in the root directory of the wedding website
* see what files you've modified: `git status`
* type `git add .` into the terminal to let it know what files you're updating
* type `git commit -m '<brief description of changes>'` to save those changes into Git's system on your local computer
* DEPLOYING TO LIVE WEBSITE: type `git push`
