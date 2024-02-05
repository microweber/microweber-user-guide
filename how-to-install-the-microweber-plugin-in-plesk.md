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

