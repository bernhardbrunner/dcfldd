<!--Last modified: 2017-04-20 22:03
  Author: Bernhard Brunner
  -->
# Bash completion for dcfldd

dcfldd did not come with a bash completion file, so i created one based on the dd
standard file. It comes with 'smart' keyword expansion for the options 
hash, hashconv, status, and sizeprobe.

# Installation

- Create a directory, e.g. `~/bin/bash_completion.d` for your custom bash_completion file or drop the file into `/etc/bash_completion.d` for system wide installation
- If you have/want to use your own bash_completion directory, add the following code to `~/.bashrc`
```bash
    if [ -d ~/bin/bash_completion.d ] ; then
      for f in ~/bin/bash_completion.d/*;
      do
        source $f
      done
    fi
```
- reload the shell and test it


