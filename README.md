NW.js does not save window size and location, this script aims to solve that by saving state using LocalStorage. I did not write the original script, I merely tweaked it.

Original source: https://github.com/nwjs/nw.js/wiki/Preserve-window-state-between-sessions  
Original contributors: https://github.com/nwjs/nw.js/wiki/Preserve-window-state-between-sessions/_history

### Prepare
You should hide the main window in ```package.json``` and let the script show it, otherwise users will see the default window size for a brief moment. 
```JSON
{
  "window": {
    "show": false
  }
}
```

### Install
```
bower install --save mccxiv/nwjs-preserve-window-state
```

### Use
```HTML
<!-- Add to main html file -->
<script src="bower_components/nwjs-preserve-window-state/winstate.js></script>
```