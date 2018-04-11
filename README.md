# SFERA web V1
# ARToolKit.js

Emscripten port of [ARToolKit](https://github.com/artoolkit/artoolkit5) to JavaScript.
Utilisation de jsartoolkit sur une page web (mozilla)
Detection des marqueurs pattern hiro et kanji 
Affichage de donuts et sphere 3D

Exemple basé sur jsartoolkit

# ARToolKit JS API

```js
<script async src="build/artoolkit.min.js">
// include optimized ASM.js build and JS API
</script>
```

# ARToolKit JS debug build

```js
<script src="build/artoolkit.debug.js">
// - include debug build
</script>
<script src="js/artoolkit.api.js">
// - include JS API
</script>
```

# ARToolKit Three.js helper API

```js
<script async src="build/artoolkit.min.js">
// - include optimized ASM.js build and JS API
</script>
<script async src="three.min.js">
// - include Three.js
</script>
<script async src="js/artoolkit.three.js">
// - include Three.js helper API
</script>
<script>
window.ARThreeOnLoad = function () {
console.log("Three.js helper API loaded");
};
if (window.ARController && window.ARController.getUserMediaThreeScene) {
ARThreeOnLoad();
}
</script>
```

