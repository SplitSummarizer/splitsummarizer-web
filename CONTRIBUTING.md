
# Contributing to SplitSummarizer

## Setup

Create a fork of the repository on your Github account. You can go this by visiting to [https://github.com/SplitSummarizer/splitsummarizer-web](https://github.com/SplitSummarizer/splitsummarizer-web) and clicking on 'Fork.' This will create a copy of the repository on your Github account.

Clone the repo on your computer to start working on it. Use 
```bash
git clone https://github.com/YOUR_USER_NAME/splitsummarizer-web ./split
```

Navigate to the folder with all the source code using

```bash
cd split
```

Set the [main repository](https://github.com/SplitSummarizer/splitsummarizer-web) as the project "upstream" this will allow you to pull in new changes before submitting your own. Use
```
git remote add upstream https://github.com/SplitSummarizer/splitsummarizer-web
```

Verify that your repo is set up properly by running `git remote -v` This should give you:

```bash
origin  https://github.com/YOUR_USER_NAME/splitsummarizer-web (fetch)
origin  https://github.com/YOUR_USER_NAME/splitsummarizer-web (push)
upstream    https://github.com/SplitSummarizer/splitsummarizer-web (fetch)
upstream    https://github.com/SplitSummarizer/splitsummarizer-web (push)
```

## Contributing code

All development happens on the `develop` branch and only production ready code is merged into `master` to start making changes, first switch to the develop branch.

```bash
git checkout develop
```

You can always check what branch you are on my running 

`git branch -v`

This should give you something similar to:

```bash
  bootstrap_modular                   a747228 Finished Bootstrap base
  bug-unicode-ascii-bug               56dac45 Fixed utf-8 encoding/decoding issue.
  clean-franken-bootstrap             26b5259 uninstall flask-bootstrap and flask-nav. update requirements.
  clean-requirements                  d4a02cf Clean virtual env.
* develop                             1d81b56 Added two column summmary output.
  frontend-contact-page-format        e015fc9 Finished contact form port
  frontend-new-web-port               9a95eb9 Restructure summarizer form
  frontend-new-web-port-styles        3bd2c60 Minor: made mast head gradient global
  frontend-summarized-view-in-columns 1d81b56 Added two column summmary output.
  master                              1d81b56 Added two column summmary output.
  reformat-output                     e2592d8 Finished reformatting.
  sumy-fix                            50652c2 installed required sumy dependencies
```

The asterisk identifies the branch you are on. 

Pull in the new changes from the main repository before you start work on your features.

```bash
git pull upstream develop
```

Once you are on the `develop` branch and have pulled in the recent changes, create a new branch where you will be working on your new feature. Use

```bash
git checkout -b your-new-feature
```

Make sure to replace `your-new-feature` with something that identifies the feature you want to work on. If, for instance, you want to change the website theme to a dark teal instead of the current purple, you can call your branch `frontend-base-color-change`, etc.

Work on your changes and commit changes as required.

## Incorporating changes

Push your branch to Github

```bash
git push origin your-new-feature
```

You will asked to enter your github.com credentials to finish pushing the changes, so do that.

Once done, you can now visit your repository on Github using your browser. Click on the "Compare and pull request" and add details about your new feature.

You're done! Once you finish making the pull request, the [maintainer](http://www.github.com/abhikpal/) of the repository will be notified and your changes will be merged into the main code base!
