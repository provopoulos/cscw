<h2 align="center">Mobile and Social Media</h2>

#### Vasileios Provopoulos | ID/RN: P2018017 | p18prov@ionio.gr
<h2 align="center">Phase #1</h2>

### DOKEY: [#CSCW](https://github.com/courses-ionio/dokey#cscw)
|           1st           |                   Deliverables                   |                             Asciinema                            |  Deadline  |  Commit  |
|:-----------------------:|:------------------------------------------------:|:----------------------------------------------------------------:|:----------:|:--------:|
| Upload and share files. | Manage your cloud storage from the command line. | [dbxheadless](https://asciinema.org/a/Fgq91gACiXka5sEqOAWVx66nA) | 30/03/2020 | &#x2611; |

Dropbox Headless works as a background [daemon](https://www.dropbox.com/install) service on Linux and can be controlled by a Python script from the command line. User-wide installation is useful so as to avoid providing the full path every time the script executes.
```console
[p18prov@P2018017 ~]$ ls /usr/local/bin/
dropbox.py
```

|         2nd        |                                       Deliverables                                      |                           Asciinema                          |  Deadline  |  Commit  |
|:------------------:|:---------------------------------------------------------------------------------------:|:------------------------------------------------------------:|:----------:|:--------:|
| Check the weather. | Fetch weather forecast with enhanced search capabilities and export to desired formats. | [wttr.in](https://asciinema.org/a/NRX9Aaf2UVoC3ItM2W7QNBo0k) | 30/03/2020 | &#x2611; |

|                  3rd                  |                                 Deliverables                                |                         Asciinema                        |  Deadline  |  Commit  |
|:-------------------------------------:|:---------------------------------------------------------------------------:|:--------------------------------------------------------:|:----------:|:--------:|
| Connect to a remote machine with SSH. | Connect to a remote machine from local computer and perform previous tasks. | [ssh](https://asciinema.org/a/aqMWtB1zOEuUIq0hg6wiGhyUg) | 30/03/2020 | &#x2611; |

|                 4th                 |                                                    Deliverables                                                   |                          Asciinema                         |  Deadline  |  Commit  |
|:-----------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------:|:----------:|:--------:|
| Back up your home directory online. | Keep directories synchronized across different locations, back up home directory and automate this whole process. | [rsync](https://asciinema.org/a/6pRQQn8T7j3XBtcvTdKT3M7dr) | 30/03/2020 | &#x2611; |

Tasks #3 and #4 can be used in tandem to keep our directories/files synchronized. Below is an overview of the most useful commands.
```console
$ rsync -avhP -e "ssh -p xxxx" FROM_LOCALorEXTERNAL_PATH username@host:TO_REMOTE_PATH
$ rsync -avhP -e "ssh -p xxxx" username@host:FROM_REMOTE_PATH TO_LOCALorEXTERNAL_PATH
$ rsync -avhP --exclude=".[!.]*" -e "ssh -p xxxx" username@host:FROM_REMOTE_PATH TO_LOCALorEXTERNAL_PATH
$ rsync -avhP --exclude=".[!.]*" --exclude-from="exclude.txt" "$HOME"/ TO_EXTERNAL_PATH
$ crontab -e
30 10 * * * rsync -avhP --exclude=".[!.]*" --exclude-from="exclude.txt" --delete "$HOME" TO_EXTERNAL_PATH
```

### Collaborative-DEV: [#MINIMAL-IONIO](https://github.com/ioniodi/minimal-ionio), [#SITE-GR](https://github.com/ioniodi/site-gr)

| Difficulty |                        Issue                        |                         PR                        |                            Demo                           |
|:----------:|:---------------------------------------------------:|:-------------------------------------------------:|:---------------------------------------------------------:|
|  Very Easy | [#36](https://github.com/ioniodi/site-gr/issues/36) | [#37](https://github.com/ioniodi/site-gr/pull/37) |                          &#9744;                          |
|    Easy    | [#81](https://github.com/ioniodi/site-gr/issues/81) | [#86](https://github.com/ioniodi/site-gr/pull/86) | [7c8c65](https://cranky-kare-7c8c65.netlify.app/courses/) |

<h3 align="center">End of: Phase #1</h3>

<h2 align="center">Phase #2</h2>

### Collaborative-DEV: [#MINIMAL-IONIO](https://github.com/ioniodi/minimal-ionio), [#SITEGR](https://github.com/ioniodi/sitegr), [#SITE-GR](https://github.com/ioniodi/site-gr) (Archived)

|   Difficulty  |                                                   Issue                                                   |                                                           PR                                                           |                              Demo                              |                                      Wiki                                     |                                                                                                                          Branches                                                                                                                         |
|:-------------:|:---------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| Medium - Hard |                            [#83](https://github.com/ioniodi/site-gr/issues/83)                            | MI: [#23](https://github.com/ioniodi/minimal-ionio/pull/23)<br>SG: [#105](https://github.com/ioniodi/site-gr/pull/105) |     [753ac0](https://vibrant-albattani-753ac0.netlify.app/)    | [Embedded Timeline](https://github.com/ioniodi/sitegr/wiki/Embedded-Timeline) | [provopoulos/minimal-ionio@twitter_module](https://github.com/provopoulos/minimal-ionio/blob/twitter_module/_includes/twitter-module.html)<br>[provopoulos/site-gr@twitter_module](https://github.com/provopoulos/site-gr/blob/twitter_module/index.html) |
|      Hard     | [#1](https://github.com/ioniodi/sitegr/issues/1)<br>[#124](https://github.com/ioniodi/site-gr/issues/124) |    MI: [#34](https://github.com/ioniodi/minimal-ionio/pull/34)<br>SG: [#3](https://github.com/ioniodi/sitegr/pull/3)   | [d9174b](https://practical-minsky-d9174b.netlify.app/contact/) |        [Maps](https://github.com/ioniodi/sitegr/wiki/Embedded-Timeline)       |           [provopoulos/minimal-ionio@ds_maps](https://github.com/provopoulos/minimal-ionio/blob/ds_maps/_includes/communication-info.html)<br>[provopoulos/sitegr@ds_maps](https://github.com/provopoulos/sitegr/blob/ds_maps/_data/contact.yml)          |

<h3 align="center">End of: Phase #2</h3>
