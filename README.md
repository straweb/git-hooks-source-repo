# git-hooks-samples-repo

# What are hooks?

Hooks are scripts that help you enforce policies on your repository by triggering scripts at certain events that enforce policies such as 'The commit message must be longer than 20 characters' or 'The test suite must be run before a commit and if it fails, reject the commit'.

Hooks are available in every VCS I have used before. They are also available in Visual Sourcesafe which is not a VCS.

# Git Hooks

In Git the hook scripts can be implemented using any language but Shell, Ruby, Perl and Python scripts are the most common as far as I know.

The language of the script is determined by the shebang notation as it is usually in Linux based software. Note that this also applies to Windows because Git for Windows runs under MSYS.

If you supply the --no-verify argument to the git command then the command will still be executed even if one (or more) of the hooks failed (i.e. returned a non-zero status code). Please do this only if you know what you are doing.

These hooks reside under the .git/hooks/ directory of your repository.

The Git-SCM book already covered the various hooks available. It also provided an example of how those hooks can be written in Ruby.

For a quick reference you can open your favorite shell and type:

git hooks --help

# Why do you need git hooks in your project?
Hooks are little scripts you can place in `$GIT_DIR/hooks` directory to trigger action at certain points.

They are very powerful and helpful.

You can do a lot of things with them:

  * [Validate code](http://jshint.com/) and run tests before commit.
  * [Check codestyle](http://jscs.info/).
  * Spell check the commit message or check it format.
  * and etc.


# Supported platforms
  * Unix
  * macOS
  
# Contributing
We love contributions, be they bug reports, feature ideas, or pull requests. See our guidelines for contributing to best ensure your thoughts, ideas, or code get merged.

# License
This project is released under the MIT license.



  
