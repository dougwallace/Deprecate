# Deprecate

### Problem:
Creating a way to mark files and directories deprecated within a codebase
Sometimes we are stuck with legacy code or technical debt. As a newcomer to a large codebase it can be a bit confusing.

This script is meant to be used as a git pre-commit hook to warn developers of deprecated code before committing.

### Try it out

1. Create a new dir somewhere and initialize a git repo.

2. Add some files and directories for testing purposes.

3. Create a file named ".deprecate" in the root of the repository.

  - Add file names like so **"f: path/from/root/to/filename.exp"**


  - Add directories like so **"d: path/to/dir"**

4. Copy the executable into your **.git/hooks** dir and rename it **"pre-commit"**

5. Use git add to add some deprecated files to your staging area. Try to commit

6. Try unstaging those files and use git add to add files or directories not on the list and try to commit.

### Improvements: 
I'd like to work on creating a deprecate command that you can run within a directory to add files or directories to the .deprecate file's list.

I'd also like the command to be able to list all of the files, search for deprecated filenames and directory names, and some other basic features.
