# Useful Teminal Commands

## Mac
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
```
# Install brew packages
brew install yarn
brew install node
brew install tmux
brew install rbenv
brew install ruby-build
brew install overmind
brew install postgresql

# Install gems
gem install pg

# RVM or RBENV
rbenv install 3.0.2 # install specific version
rbenv global 3.0.2 # set global ruby version
rbenv local 3.0.2 # set global ruby version
rbenv rehash
# Add this line to ~/.zshrc for RBENV
eval "$(rbenv init -)"

# Restart terminal/vscode
sudo gem update
sudo gem install rails

# Turn off AirPlay Reciever in System settings under Sharing
yarn
bundle install
rails db:setup
rails db:migrate
overmind start -f Procfile.dev
```