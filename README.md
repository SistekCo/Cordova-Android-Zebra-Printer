Cordova-Bluetooth-Printer-Plugin
================================

Cordova Bluetooth Printer Plugin for android

This is a Cordova plugin that allows you to print to Zebra bluetooth printers using your Android device.

Installation: cordova plugin add https://github.com/SistekCo/Cordova-Android-Zebra-Printer


#AndroidPrinter = {

    list: function (fnSuccess, fnError) {
        exec(fnSuccess, fnError, "BluetoothPrinter", "list", []);
    },
    open: function (fnSuccess, fnError, name) {
        exec(fnSuccess, fnError, "BluetoothPrinter", "open", [name]);
    },
    close: function (fnSuccess, fnError) {
        exec(fnSuccess, fnError, "BluetoothPrinter", "close", []);
    },
    print: function (fnSuccess, fnError, printer, message) {
        exec(fnSuccess, fnError, "BluetoothPrinter", "print", [printer, message]);
    }
};
