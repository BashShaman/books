# Notes

1.  git-bash-prompt is a script to display information related to git inside your prompt.

1.  Git cares about the permission to execute the file for the owner.  
    If this permission is changed, you should stage the file and comit it.
 
1.  Windows filesystems don't have separate permissions to execute files.  
    If the file can be read, it can be executed.  
    If the filesystem doesn't have separate permissions for execution,  
    `git config core.filemode false` will be set.
    
1.  Git doesn't see empty directories. So an empty directory cannot be added to index or committed.  
    Put an empty `.gitkeep` file to make an empty directory visible to Git.

1.  `./.git/config`

    Path to the file with local configurations.  
    These are configurations for a particular repository.  
    Use the flag `--local` to set or don't use any flag at all (default value).
    
1. ` ~/.gitconfig`

    Path to the file with global configurations.  
    These are configurations for all repositories of the user.  
    Use flag `--global` to set.
    
1.  `/etc/gitconfig`

    Path to the file with system configurations.
    These are configurations for all users of the system.  
    Use flag `--system` to set.
    
1.  Search order for a particular configuration: local -> global -> system.
