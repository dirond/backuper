# backuper

Systemd service unit and program that create archived copy of files from specified directories.  
Created archives encrypt by gpg (symmetric or public key) and may be upload to [disk.yandex.ru](https://disk.yandex.ru) via REST API  
Auth token for uploading may be recieved from [oath.yandex.ru](https://oauth.yandex.ru/authorize?response_type=token&client_id=291365530235416bb346ae0286a9375e)  


## Installation

Read Installation.txt

## Use

run manually or copy `backuperd.service` file to `/etc/systemd/system` and run `sudo systemctl enable backuperd.service`

## TODO

1. Add `install.sh`
2. Add systemd timer unit (now the service is started either at system startup or manually)
2. Add file syncronization between local storage and cloud (in case when backup was been created but not uploaded to the cloud)
3. Add options:  
	`--show-config`  
	`--show-files-to-backup`  
	`--show-files-to-exclude`  
	`--last-status`  
	`--add-files`  
	`--exclude-files`  
	`--gui-notifications=[yes|no]`  
	`--symmetric=[yes|no]`  
	`--upload-to-yandexdisk=[yes|no]`  
	`--set-gpg-key-email`  
