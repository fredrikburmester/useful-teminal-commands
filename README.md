# Useful Teminal Commands

## Mac
### Python
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

