

	## OS Packages
	
	<details><summary>APT Repositories</summary>
	
	#### ansible

	```shell
	  def foo
		puts 'bar'
	  end
	```
		
	#### docker

	```shell
	  def foo
		puts 'bar'
	  end
	```
		
	#### opera

	```shell
	  def foo
		puts 'bar'
	  end
	```
		
	#### google-chrome

	```shell
	  def foo
		puts 'bar'
	  end
	```
		
	#### Plex

	```shell
	  def foo
		puts 'bar'
	  end
	```

	</details>
	
### test 

<details><summary>OS PAckages</summary>

	### cron
	####Download Perms
	### fail2ban
	#### SSH Jail
	#### Scripts
	##### Check IP Banned
	##### Unban IP
	### iptables
	### QEMU/KVM
	#### Windows
	#### OSX
	### nfs-kernal-server
	### rsyslog
	### ssh
	### sudoers
	### /etc/skel
	### UFW
	#### GUFW
	###   X11
	#### xfce4
	###   XRDP	
	
</details>
		3rd Party 
		Packages

		  Docker

			Config

			Compose

			  Networking

				proxy

			  Services

				Portainer

				Proxy

				OpenVPN

				Pi-Hole

			  Portal

				OMBI

				qBittorrent

				Radarr

				Sonarr

				Jackett

			  common-config
			restart: always
			networks:
			  - proxy
			dns:
			  - 8.8.8.8
			environment:
			  - PUID=666
			  - PGID=666
			  - TZ="Europe/London"
			  - VIRTUAL_HOST=<service>.pknw1.co.uk
			  - VIRTUAL_PROTO=https
			volumes:
			  - /etc/localtime:/etc/localtime:ro
			  - ./config/<service>:/config
			  - /shared:/shared
			  - /download:/download
			  - /content:/content
			  - /tmp:/tmp
			restart: unless-stopped

		  webmin

			Additional Modules

			  iPhone Theme

			  VM Manager

		  Plex Media Server

		  HAProxy

			Config

			Scripts

			  check-config

		  ansible

			server-base

			portal-base

		USer and Groups
