# textChange
A custom jQuery event for inputs and textareas.

Exposes an event called "textChange" which is triggered 2 seconds after user stops typing into an input or textarea. This is useful when you want to catch a text change before the input goes out of focus, but not on every single keystroke.

It works just like you would expect, even includes a shortcut method.

    $("#textbox").on("textChange", function(){
    	console.log($(this).val());
    });
    
    $("#textbox2").textChange(function(){
    	console.log($(this).val());
    });
    
See: https://jsfiddle.net/tfr91xky/
