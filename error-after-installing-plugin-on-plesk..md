---
description: https://github.com/microweber-dev/plesk-plugin
---

# Error after installing Plugin on Plesk.

### How to install the plugin

1. Open Plesk Panel
2. Go to Extensions Catalog and install "Panel.ini Editor"
3. Open the Panel.ini Editor
4. Add these lines & save

```
[license]
fileUpload=true

[ext-catalog] 
extensionUpload = true

[php] 
settings.general.open_basedir.default="none"
```

#### Uploading

After activation of `extensionUpload` go to Server Management > Extensions

Then upload the zip file fron the upload button

<figure><img src="https://camo.githubusercontent.com/a8768f9c6af40c6112e0cd8c1a7b80622511f6a97bdf607b42446000b4abc9d7/68747470733a2f2f6d6963726f77656265722e636f6d2f63646e2f706172746e6572732f706c65736b2f75706c6f61645f657874656e73696f6e2e706e67" alt=""><figcaption></figcaption></figure>

### How to use

**For automatic install**: In order to make automatic install when the user creates new domain, you must go to _Home->Service Plans->Hosting Plans_ and then click on _Additional Services_ and select _Install Microweber_ from the dropdown box.

<figure><img src="https://camo.githubusercontent.com/5cdd7899f4edbb39c9e9a9a1d229b33368f7dee4225cb0b2722418a6651858d8/68747470733a2f2f6d6963726f77656265722e636f6d2f63646e2f706172746e6572732f706c65736b2f706c616e2e706e67" alt=""><figcaption></figcaption></figure>

**For manual install**: Click the Microweber icon in the sidebar under _Server management->Microweber_ and then click on _Install_ and select _Domain_ from the dropdown box.

<figure><img src="https://camo.githubusercontent.com/3e42b5a6e44a6ffeeee90e2bfa0e7ff50f2104d6898223e1a6bf66017efcf9e7/68747470733a2f2f6d6963726f77656265722e636f6d2f63646e2f706172746e6572732f706c65736b2f696e7374616c6c2e706e67" alt=""><figcaption></figcaption></figure>

### Settings

**For plugin setup**: Go to _Server management->Microweber->Settings_ and you will be able to set various options of the plugin and also connect it to WHMCS.

<figure><img src="https://camo.githubusercontent.com/592a9845954a685899c1c2be2606716b41ea5c25164c8482439922419ba83340/68747470733a2f2f6d6963726f77656265722e636f6d2f63646e2f706172746e6572732f706c65736b2f73657474696e67732e706e67" alt=""><figcaption></figcaption></figure>

### Templates download and Updates

**For templates setup**: Go to _Server management->Microweber->Versions_ and you will be able update the plugin and download templates

<figure><img src="https://camo.githubusercontent.com/6c95f5e9805ee196bb707ba505fc9066d97d98d654c50549d1bc6533ac71fc21/68747470733a2f2f6d6963726f77656265722e636f6d2f63646e2f706172746e6572732f706c65736b2f76657273696f6e732e706e67" alt=""><figcaption></figcaption></figure>

### Web server setting

If your server is slow you can improve the speed by editting some server setting

#### Nginx setting

* open the created /etc/nginx/conf.d/directives.conf file in a text editor

```
nano /etc/nginx/conf.d/directives.conf
```

* Add required directives. For example:

```
proxy_buffer_size          128k;
proxy_buffers              4 256k;
proxy_busy_buffers_size    256k;
```

#### Folders where the plugin are installed

Folders where the plugin will be installed:

```
/opt/psa/admin/sbin/modules/microweber
/usr/local/psa/admin/plib/modules/microweber
/usr/local/psa/admin/share/modules/microweber
/usr/local/psa/var/modules/microweber
```
