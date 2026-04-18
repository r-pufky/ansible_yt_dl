# youtube-dl
Download youtube videos.

## Requirements
This role **only** syncs entire user channels. No additional requirements.

## Role Variables
Settings have been throughly documented for usage.

[defaults/main.yml](https://github.com/r-pufky/ansible_youtube_dl/blob/main/defaults/main/main.yml).

## Dependencies
N/A

## Example Playbook
host_vars/youtubedl.example.com/vars/youtube_dl.yml
``` yaml
youtube_dl_download_dest: '/data/youtube'
youtube_dl_users:
  - 'username_of_channel_to_sync'
```

site.yml
``` yaml
- name:   'youtube-dl server'
  hosts:  'youtubedl.example.com'
  become: true
  roles:
     - 'r_pufky.youtube_dl'
```

## Issues
Create a bug and provide as much information as possible.

Associate pull requests with a submitted bug.

## License
[AGPL-3.0 License](https://github.com/r-pufky/ansible_youtube_dl/blob/main/LICENSE)

## Author Information
https://github.com/r-pufky
https://keys.openpgp.org/vks/v1/by-fingerprint/466EEC2B67516C7117C85CE3A0BC35D16698BAB9
