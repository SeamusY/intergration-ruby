# Introduction
This is a simple ruby application for website testing, that does not require to write the test cases. The test cases is based upon the feature folder directly, reducing work development time.

# Prerequisite
- Ruby (After installing rbenv)
- [HomeBrew](https://brew.sh/)
- [rbenv](https://github.com/rbenv/rbenv)

Note: These instructions are refering to the bash methods, any other methods such as .zshrc or bash .bashrc, may not be covered in this instructions.

# Instructions
Follow these commands:
<br/>
Install [HomeBrew](https://brew.sh/)
```bash
brew install rbenv
nano ~./bash_profile
insert 'eval "$(rbenv init -)"' into file
```
Close Terminal and Restart Terminal | source 

```bash
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash

```
If all command run correctly you will see:
```
Checking for `rbenv' in PATH: /usr/local/bin/rbenv
Checking for rbenv shims in PATH: OK
Checking `rbenv install' support: /usr/local/bin/rbenv-install (ruby-build 20170523)
Counting installed Ruby versions: none
  There aren't any Ruby versions installed under `~/.rbenv/versions'.
  You can install Ruby versions like so: rbenv install (Your version number)
Checking RubyGems settings: OK
Auditing installed plugins: OK

```
Conintue:

```
brew upgrade ruby-build
rbenv install -l
rbenv install (Ruby version Anything above 2.3 will do)
```

# Start
```
cd to Folder with GemFile
rbenv local (your version that you choose from the earlier list)
bundle install
cucumber -p verbose
```
If you are not seeing it run correctly, please follow this set of instructions:
```
gem install cucumber-api
cucumber -p verbose
```
