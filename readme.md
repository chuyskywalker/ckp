# CKP Website

A website for [celinakayporter.com](https://celinakayporter.com).

## Development Instructions

### Setup

* Get a [github.com account](https://github.com/join).
* Download a git (version control) client. Something like [Github Desktop](https://desktop.github.com/) or the [git cli program](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

Clone the repo to your machine:

```
git clone https://github.com/chuyskywalker/ckp.git
```

### Making Changes Locally

Once the repository is on your computer, you can run `hugo` which will build the site from the markdown files and spin up a local server so you can preview your changes.

```
cd ckp
./binaries/hugo.exe -s site/ server --disableFastRender
```

Will start the local server, then simply visit [http://localhost:1313/ckp/](http://localhost:1313/ckp/) to see the site.

In development mode, the site will automatically reload as you make changes to files.

### Making Local Changes Real

When you are happy with the changes you've made, you'll need to `commit` and `push` the changes back to Github.

From the cli it would look like this:

```
# Add all new files and changes files to a staging area
git add -A

# Commit all the staged changes
git commit --message "A message about the changes you've made"
```

This will save all the changes you've made as a "commit". You can now `push` your changes to Github:

```
git push origin master
```

Once the push is complete, your changes will be on github.

### Rebuilding the Real Site

You don't have to do anything! This website is integrated with [TravisCI for site builds](https://travis-ci.org/chuyskywalker/ckp). TravisCI is a free service that will create builds of the website and publish them back to Github Pages.

Github Pages is a free hosting service which the celinakayporter.com domain name points.
