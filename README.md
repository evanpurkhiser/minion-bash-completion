## Kohana Minion module Bash Autocomplete

This bash autocompletion script will complete the task names for [Kohana Minion](https://github.com/kohana/minion/) module using the `minion` bash script.

### Task caching

After completing the tasks once, the list of tasks will be cached (per minion script path) to speed up the autocompletion process. The downside of this is that is if you add more tasks your current bash session will not have the updated minion tasks in it's cache.

A simple work around to this would be to unset the cache varaible

    $ _minion_tasks_list=()

Or just reload your console

### Installation

Simply place the auto-completion script into your `/etc/bash_completion.d/ directory.

    sudo wget https://raw.github.com/EvanPurkhiser/minion-bash-completion/master/minion -P /etc/bash_completion.d/