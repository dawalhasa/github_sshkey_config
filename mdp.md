-> # Generate SSH_KEY <-
```bash
ssh-keygen -t ed25519 -C 'youremail@whatever.com'
```
-------

-> # Add your public key to your github ssh_key <-
```github
Go to setting
Click 'SSH and GPG Keys'
Clike 'New ssh key'
Provide 'Title'
Select 'authentication key' as default
Paste the your generated public key to inside the blog
and Add SSH Key
```
-------

-> # Manupulate your ssh key agent on your terminal <-
```bash
eval "$(ssh-agent -s)" 
Agent pid 7759
```
-------

-> # Add your ssh key to the env <-
```bash
 ssh-add ~/.ssh/github_key
```
-------

-> # Check SSH key with github <-
```bash
ssh -T git@github.com
Hi dawalhasa! You've successfully authenticated, but GitHub does not provide shell access.
```
-------

-> # Clone the repository direct from github <-
```bash
gh repo clone git@github.com:dawalhasa/basketball-match.git
````
