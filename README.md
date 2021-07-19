OVGTSL Website
==============

This is the repository for the Ohio Valley Group of Technical Services Librarians main website.

## Table of Contents
- [Background](#background)
- [Project Boards](#project-boards)
- [OVGTSL Website Technologies](#ovgtsl-website-technologies)
- [Contributing Code](#contributing-code)

## Background

This site was developed by the 2021 OVGTSL Board based upon the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) design by [Michael Rose](https://github.com/mmistakes). A great deal of organizational info can be found on the [OVGTSL Website](http://ovgtslibrarians.org/). This site should serve as a gateway to the various sources of OVGTSL information while providing visitors with a user-friendly way to find conference-specific info.

This site was designed with future users in mind, so the group chose platforms that would be accessible to a wide range of users: [Jekyll](https://jekyllrb.com) and [GitHub Pages](https://pages.github.com).

## Project Board

Active website projects and tasks are managed using Github's [kanban-style](https://en.wikipedia.org/wiki/Kanban_(development)) project boards. The website improvement plans for 2021-2022 are on the [OVGTSL Website Improvements Project Board](https://github.com/OVGTSL/ovgtsl.github.io/projects/1).

## OVGTSL Website Technologies

There are a number of technologies behind the OVGTSL website.

- [Jekyll](https://jekyllrb.com) is a Ruby gem that generates static websites from markdown, HTML, and other formats. See the [official Jekyll documentation](https://jekyllrb.com/docs/home/) for details.
- [GitHub Pages](https://pages.github.com/) is a static site hosting service that takes HTML, CSS, and JavaScript files straight from a repository on GitHub, optionally runs the files through a build process, and publishes a website.
- [GoDaddy Managed DNS](https://www.godaddy.com/help/manage-dns-records-680), or Domain Name System, converts the domain you typed into your browser to a computer-readable IP address.

## Contributing Code

Before you'll be able to locally build the website and test changes, you'll need to set up a development environment.

Pre-requisites:
- A Package Manager
  - For macOS, [Homebrew](https://brew.sh/) is popular
  - For Windows OS, try [Chocolatey](https://chocolatey.org/)
- Version Control Software
  - We're using [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- The [Ruby](https://www.ruby-lang.org/en/documentation/installation/) programming language installed
- and... the [Jekyll](https://jekyllrb.com/docs/installation/) gem

### Setup

1. ```git clone``` the [repo](https://github.com/OVGTSL/ovgtsl.github.io.git) from GitHub
2. cd to repo root and ```git pull```
3. ```bundle install```
4. Continue with step 3 below

### Contributing

The following example uses "issue#3" as a subject. That's the branch name and is used in the commit message.

1. Make sure you're on the main branch
   - ```git checkout main```
2. Make sure your main branch is up to date
   - ```git pull origin main```
3. Start up jekyll
   - ```bundle exec jekyll serve```
   - Open [http://localhost:4000](http://localhost:4000) in your browser
4. Create a new branch for your changes
   - ```git checkout -b issue#3```
5. Make changes, check [http://localhost:4000](http://localhost:4000) to see your changes live
   - We strongly recommend performing an accessibility audit (e.g. [with Chrome](https://developers.google.com/web/tools/chrome-devtools/accessibility/reference)) if you've made structural or stylistic changes (not adding text content or additional posts)
6. Add your changed files
   - ```git add {changed-files}```
7. Commit your changes with a fancy message
   - ```git commit -m "fixes issue #3"```
8. Add your branch to the repo
   - ```git push --set-upstream origin issue#3```
9. Switch back to the main branch
   - ```git checkout main```
10. Go to [https://github.com/OVGTSL/ovgtsl.github.io](https://github.com/OVGTSL/ovgtsl.github.io)
11. Make a pull request base:master and compare:issue-3
12. Wait for someone to test your changes and merge the pull request
13. Do the dance of joy 🎉

### Managing Pull Requests

1. Follow steps 1 - 3 above
2. Get any remote branches
   - ```git fetch```
3. Switch to the branch in question
   - ```git checkout BRANCHNAME```
4. ```bundle exec jekyll serve```
5. Check [http://localhost:4000](http://localhost:4000) that nothing is broken
6. Merge that branch into main (easiest to manage on the GitHub site)
