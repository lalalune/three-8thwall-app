# three-8thwall-app

To run:
To run: npx http-server -S -C cert.pem


On 'touchstart' (when the user taps the screen), a THREE.Raycaster() is used to determine where the intersection with the ground (a transparent THREE.PlaneGeometry residing at a height of Y=0) occurs.  THREE.GLTFLoader() is then used to load a .glb file and place it at the tap location on the ground. The model is instantiated with a random Y-rotation and the initial scale is set to a very small value.  tween.js is then used to apply a scale-up animation to the model.
