# aframe-joystick
An aframe component for "wasd"-like motion on mobile.
Demo here: https://sour-lyric.glitch.me/

Many thanks to [@yoannmoinet](https://github.com/yoannmoinet) for creating [NippleJS](https://github.com/yoannmoinet/nipplejs). This project is 95% NippleJS with a small adaptation for A-Frame

## Usage
#### Step 1
You'll need to include the script in your project: 
```
<script src="https://cdn.rawgit.com/mrturck/aframe-joystick/master/joystick.min.js"></script>
```

#### Step 2
Second, add `id="camera"` to your camera element, 
or create a new camera entity with `id="camera"`:
```
<a-entity camera id="camera" position="0 1.6 0" look-controls wasd-controls>
```

#### Step 3
Add `joystick` to your `a-scene` element 
```  
<a-scene joystick>
```

#### Step 4 (optional, but recommended)
If you are using the `joystick` to replace VR controls, then you'll probably want to hide the `vr-mode-ui` button.
Do this by adding `vr-mode-ui="enabled: false"` to your `a-scene` element (example below):
```  
<a-scene joystick vr-mode-ui="enabled: false">
```

