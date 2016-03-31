Cordova IOS-Bluetooth-Print plugin
==================================

## Adding the Plugin to your project
Through the [Command-line Interface](http://cordova.apache.org/docs/en/3.0.0/guide_cli_index.md.html#The%20Command-line%20Interface):

```bash

cordova plugin add https://github.com/Natalia21/phoneGapIOSPrintingPlugin.git
cordova build


## Removing the Plugin from your project

cordova plugin rm intspirit.cordova.plugin.printer
```


## Using the plugin
The plugin creates the object ```window.plugin.printer```

### Printing 
You need to download/save html using fileTransfer plugin https://github.com/apache/cordova-plugin-file-transfer. Make sure you use it after deviceReady event is called.

** Below example uses print share app for printing files.
```javascript
	window.plugin.printer.print('content', {}, function() {
		console.log('success');
	}, function() {
		console.log('error');
	});

```


## License

This software is released under the [Apache 2.0 License](http://opensource.org/licenses/Apache-2.0).
