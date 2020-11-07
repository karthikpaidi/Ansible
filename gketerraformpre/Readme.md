in order to use this playbook first install the collection for brew, gloud install on your mac using following commnd

cmd: ansible-galaxy collection install community.general


once install is completed please follow the below depending on the type of shell

to see which shell use "echo $SHELL"

google-cloud-sdk is installed at /usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk. Add your profile:

  for bash users
    export CLOUDSDK_PYTHON="/usr/local/opt/python@3.8/libexec/bin/python"
    source "/usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/path.bash.inc"
    source "/usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/completion.bash.inc"

  for zsh users
    export CLOUDSDK_PYTHON="/usr/local/opt/python@3.8/libexec/bin/python"
    source "/usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/path.zsh.inc"
    source "/usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/completion.zsh.inc"

  for fish users
    set -g -x "CLOUDSDK_PYTHON" "/usr/local/opt/python@3.8/libexec/bin/python"
    set -g fish_user_paths "/usr/local/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/path.fish.inc" $fish_user_paths