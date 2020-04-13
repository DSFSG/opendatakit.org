# ODK Website

![Platform](https://img.shields.io/badge/platform-Jekyll-blue.svg) [![Ruby version](https://img.shields.io/badge/ruby-blue.svg)](https://www.ruby-lang.org/en/downloads/) [![License](https://img.shields.io/badge/license-CC%20BY%204.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/) [![Build status](https://circleci.com/gh/opendatakit/website.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/opendatakit/website/) [![Slack status](http://slack.opendatakit.org/badge.svg)](http://slack.opendatakit.org/)

This repository is home to the [ODK homepage](https://opendatakit.org/).

## Table of Contents

* [Installing requirements](#installing-requirements)
	* [MacOS, Linux](#macos-linux)
	* [Windows](#windows)
* [Running the website](#running-the-website)
* [Contributing](#contributing)
* [Troubleshooting](#troubleshooting)

## Installing requirements

The ODK website is built with [Ruby](https://www.ruby-lang.org/en/downloads/) and below are the installation steps we recommend for getting a Ruby environment that will work best with the ODK website.

### MacOS, Linux

1. Installing `rbenv`

	**MacOS**: Installation instructions using Homebrew can be found in the [`rbenv` documentation](https://github.com/rbenv/rbenv#homebrew-on-macos). This is the preferred method for MacOS. To install `rbenv` without Homebrew, refer to the Linux instructions.

	**Linux**: The [`rbenv-installer`](https://github.com/rbenv/rbenv-installer#rbenv-installer) is a script which idempotently installs or updates `rbenv` on your system.

2. Installing Ruby

	Once `rbenv` has been installed, install the latest Ruby (currently `2.6.3`):
	```
	rbenv install 2.6.3
	```

### Windows

1. Windows users should use [RubyInstaller](https://rubyinstaller.org/).

## Running the website

1. Follow the instructions in the [contribution guide](https://github.com/opendatakit/website/blob/master/CONTRIBUTING.md) to [fork](https://help.github.com/articles/fork-a-repo/) the website repository and then [clone](https://help.github.com/articles/cloning-a-repository/) your fork.

2. Configure your project to use the correct version of Ruby.

	a. Navigate to the root directory of your project. If you use Windows, replace the `cd` command with `dir`.

	```
	cd /MY/DEVELOPMENT/DIRECTORY/website
	```

	b. Set the local application-specific Ruby version by using [`rbenv-local`](https://github.com/rbenv/rbenv#rbenv-local).

	```
	rbenv local 2.6.3
	```

	c. Verify that your project is using Ruby version `2.6.3`:
	```
	ruby -v
	```

3. Install `bundler`.
```
gem install bundler
```

4. Install this project.
```
bundle install
```

5. Launch the server. The site will update as changes are made.
```
bundle exec jekyll serve
```

## Contributing

One quick way to contribute is to review the [website](https://opendatakit.org) and [file issues](https://github.com/opendatakit/website/issues) documenting the problems you see. If you would like to help fix those issues, see [the contribution guide](CONTRIBUTING.md).

## Troubleshooting

### Permissions

If you encounter the following error:
`You don't have write permissions for the /var/lib/gems/x.x.x directory.`
then please review the installation instructions to make use of `rbenv`.

Only root has write permissions for `/var/lib`; using `sudo` for subsequent `gem install` comands won't work, and changing permissions for that directory using `chmod` is considered dangerous. This issue is avoided when using `rbenv`.

### Nokogiri

[Nokogiri (鋸)](http://www.nokogiri.org/) is a Rubygem providing HTML, XML, SAX, and Reader parsers with XPath and CSS selector support.

The installation command `bundle install` tries to install `nokogiri`.

If you face following error:
	`Gem::Ext::BuildError: ERROR: Failed to build gem native extension.`

You can fix it as follows:

For Ubuntu/Debian OS:
Run the command `sudo apt-get install build-essential patch ruby-dev zlib1g-dev liblzma-dev` and try again.

If you are using any other OS, you can follow the instructions mentioned here:
http://www.nokogiri.org/tutorials/installing_nokogiri.html
