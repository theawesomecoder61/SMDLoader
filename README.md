# SMDLoader
A three.js loader used for loading SMD files (Valve Studiomdl Data). SMD files are ASCII and are used by Valve's Source Engine. You can go to [Valve's article about SMD files](https://developer.valvesoftware.com/wiki/SMD) if you want to learn more about them.

# Features
### Supported
- meshes

### Upcoming
- skinning/skeleton
- textures (VTF is propietary, and therefore any textures will need to converted to either PNG, TGA, DDS, etc.)
- animation

# How to use
1. Download the latest version of SMDLoader.js
2. In your HTML, add
```html
<script src="path/to/SMDLoader.js"></script>
```

# Examples
### Basic
```js
var loader = new THREE.SMDLoader();
loader.load("model.smd", function(object) {
  // object is either a THREE.Mesh or a THREE.SkinnedMesh (depends on whether there is a skeleton present in the SMD file)
  scene.add(object);
});
```
### Scene
[Click here to see SMDLoader in action.](http://metasciencetechnologies.com/smdloader)

# Changelog
### Version 1.0 - ??/??/2017
- initial version
- meshes are the only thing supported right now
