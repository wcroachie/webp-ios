this is a polyfill to add support for browsers that do not support the following:

HTMLCanvasElement.toDataURL("image/webp",quality)
HTMLCanvasElement.toBlob(blob=>{},"image/webp",quality)

It uses webassembly and the module pulled from the "examples" folder in the chromium source code.

it hooks the HTMLCanvasPrototype so it isn't exactly a great solution but it works until webkit decides to support webp encoding for canvases.
enjoy!
