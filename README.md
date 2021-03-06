# WorkshopExample

[![Coverage Status](https://codecov.io/gh/Samreay/WorkshopExample/branch/master/graph/badge.svg)](https://codecov.io/gh/Samreay/WorkshopExample)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/ea7ca374a79c4321952715a228a454f0)](https://www.codacy.com/app/samuelreay/WorkshopExample?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Samreay/WorkshopExample&amp;utm_campaign=Badge_Grade)
[![Build Status](https://img.shields.io/travis/Samreay/WorkshopExample.svg)](https://travis-ci.org/Samreay/WorkshopExample)
[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/Samreay/blob/master/LICENSE)

A small github repo used as an example for the coding workshop!

### [Access the online doco here!](http://samreay.github.io/WorkshopExample)

-----------

To use this framework you will need to:


1. Replace my email (samuelreay@gmail.com) with your own.
2. Replace all instances of samreay & samuelreay, with your own username (case insensitive replace).
3. Replace my name (Samuel Hinton) with yours (used in the doc and license).
3. Update the project name if you rename it. (At this point, should have edits to .travis.yml, setup.py, README.md, conf.py, LICENSE.)
4. Enable Travis, CodeCov and Codacy. (You may need to make a commit and push after enabling travis to kick off a build.)
5. Update the codacy badge in this readme because it uses more than username/repo (get the badge from codacy project settings).
6. Set an environment variable in travis called GITHUB_API_KEY with a Personal Access Token to commit Sphinx html to public repos.

Steps for how this project was set up can be found in the `Presentation.pdf` file in this repository, which was 
presented in December 2017 for the CAASTRO Code Workshops.

-----------

With Travis, CodeCov and Codacy set up, tests will run, cod style will be analyses, and documentation rebuilt, on each commit.

If you do not enable travis, you can run the tests your self by running (in the top level directory):

`pytest -v --cov=.` for \*nix, and `python -m pytest -v --cov=.`

You can build documentation yourself by navigating to the `doc` directory, and running `make clean && make html`, which will build the HTML builds in the `doc/_build/html` directory. Open `index.html` in that directory to see the documentation. 
