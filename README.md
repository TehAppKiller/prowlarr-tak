# prowlarr-tak
[![prowlarr-tak](https://snapcraft.io/prowlarr-tak/badge.svg)](https://snapcraft.io/prowlarr-tak)

## Snap Description
Canonical Snap for Prowlarr\
https://snapcraft.io/prowlarr-tak

## Prowlarr Description
Prowlarr is an indexer manager/proxy built on the popular *arr .net/reactjs base stack to integrate with your various PVR apps.
Prowlarr supports management of both Torrent Trackers and Usenet Indexers. 
It integrates seamlessly with Lidarr, Mylar3, Radarr, Readarr, and Sonarr 
offering complete management of your indexers 
with no per app Indexer setup required (we do it all).

See https://prowlarr.video for more details.

## Information

The web interface is accessible by default at http://localhost:9696

Prowlarr Release 1+\
Core20 is still required for dependencies\
Service is restarted on any condition.

Post install commands required to access media folders and see resources :
```
sudo snap connect prowlarr-tak:removable-media
sudo snap connect prowlarr-tak:mount-observe
```

Post install commands required to access home folder :
```
sudo snap connect prowlarr-tak:home
```
**!!! Files can only be written in a directory owned by 'root' !!!**\
This is due to current behavior and restrictions of snaps running as daemon by Canonical.

## FAQ
See my common doc about [FAQ](https://github.com/TehAppKiller/Snapcraft-common-doc/tree/main#FAQ).

## Building
The snap requires Core20 for .NET Radarr source dependencies.\
See my common doc about [building a snap](https://github.com/TehAppKiller/Snapcraft-common-doc/tree/main#Building).
## Versionning
See my common doc about [versionning](https://github.com/TehAppKiller/Snapcraft-common-doc/tree/main#Versionning).
