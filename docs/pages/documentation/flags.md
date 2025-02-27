# flags
<h4 class="fw-light">Highly-specific options that don't deserve their own configuration option</h4><br/>

### **What are flags?**
Flags allow for enabling/disabling possibly advanced features that don't have their own option in your [conf.yml](?page=documentation/confyml) file. Multiple flags must be seperated with comma's.

<br/>

### **Flags**

##### Feature-specifc flags
`ignorePlaceholders`\
Skip applying placeholders. This improves installation speed for extensions with a lot of files, but is generally not recommended.

`ignoreAlphabetPlaceholders`\
Skip applying alphabet (a-z, _) placeholders. This is automatically disabled when placeholders are disabled.

<br/>

##### Advanced flags
`hasInstallScript`\
Right before the installation completes, extensions with this flag will be able to run a shell script. This script must be called "install.sh" and be in the root of your data directory.

`hasRemovalScript` <span class="badge bg-primary-subtle text-primary-emphasis rounded-pill">Developer branch</span>\
Right before starting the extension removal process, extensions with this flag will be able to run a shell script to undo some changes Blueprint isn't able to. This script must be called "remove.sh" and be in the root of your data directory.

<br/>

##### Developer flags
`developerIgnoreInstallScript`\
Ignore the custom extension installation script when installing your extension through developer commands.