### Notice:

**You can use this visual builder to create templates and submit PRs to this repo if they work: [Shipwright](https://shipwright.yacht.sh) it's currently pretty early in development but should be able to take portainer templates (that don't have type 2 or 3 templates) and import them for editing.**

Currently most of my dev time is being spent on [Yacht](https://github.com/SelfhostedPro/Yacht/tree/vue) if you would like something added please consider making a pull request with your addition and I'll work on getting it added when I'm able to. Information about how to structure a block (for an app) is available [here](https://portainer.readthedocs.io/en/stable/templates.html) and there is a gui builder [here](https://shipwright.yacht.sh)

# Portainer Templates for Selfhosted Projects/Homelabs

This is a template focused on helping people spin up selfhosted services using Portainer and Yacht.
## Versions

The following table shows the corresponding url to use for the application you're using.

| Application  | URL |
| ------------- | ------------- |
| Yacht | https://raw.githubusercontent.com/SelfhostedPro/selfhosted_templates/master/Template/yacht.json |
| Yacht (arm) | https://raw.githubusercontent.com/SelfhostedPro/selfhosted_templates/master/Template/yacht-arm.yml |
| Portainer v1 (no OMV)  | https://raw.githubusercontent.com/SelfhostedPro/selfhosted_templates/master/Template/portainer-v1.json  |
| Portainer v2 (no OMV)  | https://raw.githubusercontent.com/SelfhostedPro/selfhosted_templates/master/Template/portainer-v2.json  |
| Portainer v1 OMV | https://raw.githubusercontent.com/SelfhostedPro/selfhosted_templates/master/Template/omv-v1.json |
| Portainer v2 OMV | https://raw.githubusercontent.com/SelfhostedPro/selfhosted_templates/master/Template/omv-v2.json|


### Prerequisites

1. A server/NAS with docker installed
2. A Portainer/Yacht setup.

*Want something we don't have? Make an issue and we'll work on adding it*

### Installing

1. Login to the Web-UI for the corresponding project.
2. Navigate to the relevant area to add a template (in Portainer v1 you'll need to enable external templates, in v.2.1.1 onwards you need to overwrite the existing app template URL of `https://raw.githubusercontent.com/portainer/templates/master/templates-2.0.json` with the relevant one above)
3. Add the template URL corresponding to the application you're using in the table above.

### Information
All templates are already configured to bind mount to various places on your drive. This branch works without the need for OMV. The following folders are all created in /portainer/

* **Files** - General file storage.
  * **AppData** - Subfolder where application data (unrelated to served data) is stored.
    * **Config** - Subfolder where configuration files for every container are stored.
* **Downloads** - Where bittorrent and usenet downloaders download files to.
* **TV** - Where tv shows are stored/moved to after downloaded.
* **Movies** - Where movies are stored/moved to after downloaded.
* **Music** - Where music is stored/moved to after downloaded.
* **Books** - Where books are stored/moved to after downloaded.
* **Comics** - Where comics are stored/moved to after downloaded.
* **Podcasts** - Where podcasts are stored/moved to after downloaded.
## App List

- Guacamole
- Homer
- Wikijs
- Bazarr
- Jellyfin
- Bitwarden_rs
- Pi-Hole
- Whoogle
- Mstream
- Filebrowser
- YouTubeDL-Material
- DashMachine
- Reactive-Resume
- LibreSpeed
- DeeMix
- Nginx Proxy Manager
- Organizrv2
- TiddlyWiki
- Watchtower
- transmission-openvpn
- airsonic
- beets
- booksonic
- bookstack
- calibre-web
- cardigann
- Chevereto
- codiad
- cops
- couchpotato
- daapd
- davos
- deluge
- domoticz
- duckdns
- duplicati
- freshrss
- gazee
- headphones
- heimdall
- htpcmanager
- jackett
- kodi-headless
- lazylibrarian
- letsencrypt
- libresonic
- lidarr
- lychee
- mariadb
- mcmyadmin
- medusa
- minetest
- minisatip
- musicbrainz
- muximux
- mylar
- nextcloud
- nginx
- nzbget
- nzbhydra
- ombi
- openvpn-as
- oscam
- photoshow
- piwigo
- plex
- plexrequests
- projectsend
- pydio
- qbittorrent
- quassel-core
- radarr
- resilio-sync
- rutorrent
- sabnzbd
- Seafile
- sickchill
- smokeping
- sonarr
- syncthing
- tautulli
- thelounge
- transmission
- tt-rss
- tvheadend
- ubooquity
- unifi
- webgrabplus
- znc

## Contributing

If you wish to contribute make a pull request, create an issue, or email me.

## Authors
* **NASHosted** - *Current Work*
* **SelfhostedPro** - *Current Work*
* **Jos Visser** - *Initial work* - [Qballjos](https://github.com/Qballjos)

See also the list of [contributors](https://github.com/SelfhostedPro/selfhosted_templates/contributors) who participated in this project.

## Acknowledgments

* LinuxServer.io for the old Template
* Inspiration being too lazy to create each container template manualy
