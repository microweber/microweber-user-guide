# How to install the Microweber plugin in Plesk

How to install the plugin&#x20;

Get the latest plugin version from here [https://github.com/microweber-dev/plesk-plugin](https://github.com/microweber-dev/plesk-plugin)

1\. Open Plesk Panel&#x20;

2\. Go to Extensions Catalog and install "Panel.ini Editor"&#x20;

3\. Open the **Panel.ini** Editor&#x20;

```
[license]
fileUpload=true

[ext-catalog] 
extensionUpload = true

[php] 
settings.general.open_basedir.default="none"
```

4\. Add these lines & save&#x20;

After that you will find the plugin in the sidebar&#x20;

<figure><img src=".gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

### How to use

After activation of `extensionUpload` go to Server Management > Extensions

Then upload the zip file from the upload button

**For automatic install**: In order to make automatic install when the user creates new domain, you must go to _Home->Service Plans->Hosting Plans_ and then click on _Additional Services_ and select _Install Microweber_ from the dropdown box.



<figure><img src=".gitbook/assets/image (6) (2).png" alt=""><figcaption></figcaption></figure>

**For manual install**: Click the Microweber icon in the sidebar under _Server management->Microweber_ and then click on _Install_ and select _Domain_ from the dropdown box.



<figure><img src=".gitbook/assets/image (1) (1) (1) (1) (2).png" alt=""><figcaption></figcaption></figure>

### Settings

**For plugin setup**: Go to _Server management->Microweber->Settings_ and you will be able to set various options of the plugin and also connect it to WHMCS.

<figure><img src=".gitbook/assets/image (2) (1) (1) (1) (2).png" alt=""><figcaption></figcaption></figure>

Templates download and Updates

**For templates setup**: Go to _Server management->Microweber->Versions_ and you will be able update the plugin and download templates

<figure><img src=".gitbook/assets/image (3) (1) (1) (1) (2).png" alt=""><figcaption></figcaption></figure>

\


\
\






