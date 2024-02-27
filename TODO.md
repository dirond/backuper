#TODO

1. Add install.sh 
2. Add systemd timer unit (now the service is started either at system startup or manually)
2. Add file syncronization between local storage and cloud (in case when backup was been created but not uploaded to the cloud)
3. Add options:
	--show-config
	--show-files-to-backup
	--show-files-to-exclude
	--last-status
	--add-files
	--exclude-files
	--gui-notifications=[yes|no]
	--symmetric=[yes|no]
	--upload-to-yandexdisk=[yes|no]
	--set-gpg-key-email
