# Useful Teminal Commands

## Mac
### Python
- Create a virtual enviroment: `virtualenv <PATH>`
- Start virtual enviroment: `source bin/activate`
- Deavtivate the virtual enviroment: `deactivate`

## UnRaid
### Nextcloud Docker
**Scan all files**
`docker exec nextcloud sudo -u abc php /config/www/nextcloud/occ files:scan --all 1> /dev/null`
