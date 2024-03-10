### Auto-generated HTML & Javascript for Cmajor Patch "vafilters"

This folder contains some self-contained HTML/Javascript files that play and show a Cmajor
patch using WebAssembly and WebAudio.

For `index.html` to display correctly, this folder needs to be served as HTTP, so if you're
running it locally, you'll need to start a webserver that serves this folder, and then
point your browser at whatever URL your webserver provides. For example, you could run
`python3 -m http.server` in this folder, and then browse to the address it chooses.

The files have all been generated using the Cmajor command-line tool:
```
cmaj generate --target=webaudio --output=<location of this folder> <path to the .cmajorpatch file to convert>
```

- `index.html` is a minimal page that creates the javascript object that implements the patch,
   connects it to the default audio and MIDI devices, and displays its view.
- `vafilters.js` - this is the Javascript wrapper class for the patch, encapsulating its
   DSP as webassembly, and providing an API that is used to both render the audio and
   control its properties.
- `cmaj_api` - this folder contains javascript helper modules and resources.

To learn more about Cmajor, visit [cmajor.dev](cmajor.dev)
