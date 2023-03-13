#Connecting to GITHUB from GIT using SSH

You can use the SSH protocol to connect and authenticate to remote servers and services.

No need to supply username and personal access token on each visit.

To setup SSH,  start Git Bash
## generate a new SSH key
  add key to ssh-agent
  add SSH key to your account on GIthub.

Check if you have any existing keys
  ls -al ~/.ssh

Lists the files in your .ssh directory, if they exist.

Generatign a new key and adding it to the ssh-agent
ssh-keygen -t ed25519 -C "your email"
Start the ssh-agent
eval "$(ssh-agent -s)"

Add key to the agent
ssh-add ~/.ssh/id_ed25519

Add the key to your github account
