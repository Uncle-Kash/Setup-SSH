Connecting to GITHUB using SSH

ussing the ssh protocol - you can connect and authenticate to remote servers and services.

No need to supply username and personal access token at each visit.

To setup SSH,
generate a new SSH key
add key to ssh-agent
add SSH key to your account on GIthub.

Check if you have any existing keys

ls -al ~/.ssh
Lists the files in your .ssh directory, if they exist.

Generatign a new key and adding it to the ssh-agent

ssh-keygen -t ed25519 -C "unclekash@pm.me"

Start the ssh-agent
eval "$(ssh-agent -s)"

Add the key to your github account