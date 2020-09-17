# LaTeX template repository for MDPI papers

[![Build Status](https://travis-ci.com/DanySK/Template-LaTeX-LMCS.svg?branch=master)](https://travis-ci.com/metaphori/Template-LaTeX-MDPI)

This repository is meant to be used as template for quickly starting MDPI papers,
having them built on a continuous integrator, and having them quickly deployed in GitHub releases.

The build system is based on Gradle, using [the latex-gradle plugin](https://github.com/DanySK/gradle-latex).

The file being built is the MDPI guide for authors.

## Using the project

1. Create a new repo using the "Use this template" button
2. Rename `instructions.tex` to your preference
2. Rename it also inside `build.gradle.kts`
3. Rename the project inside `settings.gradle.kts`
3. Further Configure the build inside `build.gradle.kts` following instructions on [https://github.com/DanySK/gradle-latex](https://github.com/DanySK/gradle-latex)
4. Test your build locally by `./gradlew buildLatex`
6. Add the `GITHUB_TOKEN` environment variable from the Travis-CI web interface `token` entry in the `deployment` section of `.travis.yml`, following [the instructions for deployment on GitHub releases provided by Travis](https://docs.travis-ci.com/user/deployment-v2/providers/releases/).
8. Just write, commit, and push, and in few minutes your files will be automagically available on GitHub.

## Contributing to the project

I gladly review pull requests and I'm happy to improve the work.
If the software was useful to you, please consider supporting my development activity
[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=5P4DSZE5DV4H2&currency_code=EUR)
