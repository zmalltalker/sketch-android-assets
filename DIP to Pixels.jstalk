// Convert a pixel value to DIP

var dips = [doc askForUserInput:"Enter a value in DIP" initialValue:100];

var msg, title;
if (dips != null){
    title = dips + "dp amounts to";
    msg = "MDPI: " + dips + "px\nHDPI: " + dips * 1.5 +  "px\nXHDPI:" + dips * 2 + "px\nXXHDPI: " + dips * 3 + "px\nXXXHDPI: " + dips * 4 + "px";
    var app = [NSApplication sharedApplication];
    [app displayDialog:msg withTitle: title];
}
