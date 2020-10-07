# One-stop .js for Android Debug Bridge (adb) over WebUSB

## Demo URL: https://niek.github.io/webadb.js/

## Usage:
```js
let webusb = await Adb.open("WebUSB");
let adb = await webusb.connectAdb("host::");
let shell = await adb.shell("uname -a");
console.log(await shell.receive());
```

#### Original repo: https://github.com/webadb/webadb.js