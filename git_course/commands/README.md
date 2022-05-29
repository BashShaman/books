# Commands

## `git config`

### Examples

1.  `git config user.name <name>`

    Set the name of the user.
     
1.  `git config user.email <email>`

    Set the email of the user.
    
1.  `git config core.editor <path-to-the-editor>`

    Set the editor to use with Git.
    
1.  `git config --global alias.c config`

    Set the alias to the `config` parameter and add it to the global configuration file.
    
1.  `git config alias.echo '!echo "Hello!"; echo "Hi!"'`

    Use '!' prefix to bind a shell command (or a sequence) with an alias.

1.  `git config -l, --list`

    List configurations from all configuration files.

1.  `git config -h`

    Get the list of options with short descriptions.
    
1.  `git config --unset <option>`

    Remove an option from the configuration file.
    
1. `git help config`

    Get detailed inforamion about the `config` parameter.
    
 ## `git add`
 
 1. `git add --chmod=+x <filename>`

    Add a file to the index and make the copy in index executable at the same time.  
    The copy inside the working tree won't be changed.
    
1.  `git add .`

    Add to the index all changes inside current directory.
    
1. `git add -A`

    Add all changes inside the working tree to the index regardless of the position inside the tree.
    
1.  `git add -f, --force <filepath>`

    Make a file from the ignored directory tracked.
    
 ## `git show`
 
1. `git show <commit-id>`

    Get the information about the commit by the id or the part of the id (at least 4 characters).
    
1. `git show <commit-id> --pretty=fuller`

    Get the information about the commiter in addition to the result of the command.
    
  ## Miscellaneous
   
1. `git update-index --chmod=+x <filename>`

    Add permissions to be executed to the index copy of a file.  
    The copy of the file inside working tree won't be changed.
    
1. `git commit --author='John Doe <johndoe@gmail.com>' --date='Sun May 29 11:09:20 2022 +0700'`

    Set the author and the date of the commit.
    
    Related environment variables:
    
    * GIT_AUTHOR_NAME
    * GIT_AUTHOR_EMAIL
    * GIT_AUTHOR_DATE
    * GIT_COMMITTER_NAME
    * GIT_COMMITTER_EMAIL
    * GIT_COMMITTER_DATE
