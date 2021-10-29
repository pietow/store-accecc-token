# store-accecc-token

## Generate Personal Access Token
1. Go to Setting
2. Go to Developer Settings
3. Go to Personal access tokens
4. Fill the form
5. Hit Generate
6. ##Install libsecret-1-0 and libsecret-1-dev
7. Use Token as the password

## Install encryption and setup

`sudo apt-get install libsecret-1-0 libsecret-1-dev`

`cd /usr/share/doc/git/contrib/credential/libsecret`

`sudo make`

Point your git credential helper to git-credential-libsecret

`git config --global credential.helper /usr/share/doc/git/contrib/credential/libsecret/git-credential-libsecret`

instead of ~~`git config --global credential.helper store`~~

## Save credentials

push, pull or clone a repo ---> when you type in your credentials it will stored encrypted in git-credential-libsecret

