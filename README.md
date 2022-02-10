# Useful Teminal Commands

## Mac
If error when running sh file 
`cat new-install.sh | tr -d '\r' > install.sh`
### Python
#### Virtual enviroments
- Create a virtual enviroment: `virtualenv <PATH>`
- Start virtual enviroment: `source bin/activate`
- Deavtivate the virtual enviroment: `deactivate`

## Homebrew 
Install homebrew: https://brew.sh/

### Homebrew Packages
- `brew install wget`
- `brew install vlc`
- `brew install rectangle`

## UnRaid
### Nextcloud Docker
**Scan all files**
`docker exec nextcloud sudo -u abc php /config/www/nextcloud/occ files:scan --all 1> /dev/null`

## Set up: Ruby on rails (m1)
Here's a quick tutorial on how to set up Rails on M1 Mac.

### Install brew packages
```
brew install yarn
brew install node
brew install tmux
brew install rbenv
brew install ruby-build
brew install overmind
brew install postgresql
```

### Install a ruby manager RVM or RBENV
```
rbenv install 3.0.2 # install specific version
rbenv global 3.0.2 # set global ruby version
rbenv local 3.0.2 # set global ruby version
rbenv rehash
```
### Install postgres client. 
If your project requires a local instance of pg then use Postgresapp:
https://postgresapp.com/

### Add this line to ~/.zshrc for RBENV
```
eval "$(rbenv init -)"
```
Remember to restart the terminal after this. 

### Install gems
**Never user sudo with gem/bundle**, and if you did, use the command below to fix any permission issues if you're using rbenv.
```
chown -R YOURUSER:staff /Users/YOURUSER/.rbenv
gem install pg
gem install rails
gem update
```

### Turn off AirPlay Reciever in System settings under Sharing
Sometimes AirPlay reciever uses the same port as rails so turning it off will solve that.

### Install the project
``` 
yarn
bundle install
rails db:setup
rails db:migrate
overmind start -f Procfile.dev
```

## GitHub
### Add SSH Keys
If you have no SSH keys: 
```
cd ~/.ssh && ssh-keygen
cat id_rsa.pub | pbcopy
```
Then paste the SSH Key on the GitHub website.
