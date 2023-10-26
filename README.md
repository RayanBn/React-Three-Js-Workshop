# React-Three-Js-Workshop

<h1>Introduction</h1>
Hi ! !<br>
Welcome to our workshop. Today we are gonna learn the basic of React ThreeJS.<br>
In order to not get lost during the Workshop, please follow the steps below.

<br>
<br>
<h2>Step 1 :</h2>
First, you need to install node !

```
sudo dnf install nodejs
```

Clone the repo ! <br><br>

```
git clone git@github.com:RayanBn/React-Three-Js-Workshop.git
```
Steps to follow for compiling :

```
npm install
```

```
npm run dev
```

<h2>Step 2 :</h2>
<br>
Let's begin by creating objects (Experience.js)<br><br>

```js
<mesh>
    <boxBufferGeometry></boxBufferGeometry>
    <meshStandardMaterial></meshStandardMaterial>
</mesh>
```

Now it's your turn to play with the object parameters to get the result you like the most !
When the object will be created, you will notice that its color won't apply.
In order to fix this issue, you have to add lights to your scene.<br><br>
https://docs.pmnd.rs/react-three-fiber/getting-started/your-first-scene#adding-lights

<h2>Step 3 :</h2><br>

Camera movement, in your canva object of the index.js file, a camera has already been added to the scene. It is up to you to learn about it and to be able to modify and manipulate it as you wish!

```js
camera={ {
    fov: 45,
    near: 0.1,
    far: 200,
    position: [ -4, 3, 6 ]
} }
```
The goal here is to be able to create a camera control, that will allow us to turn around our scene ! (OrbitControl)


<h2>Step 4 :</h2><br>

Now let's try to make the objects on our scene move. In order to interact with the objects in our scene in react, we need to use hooks.
The most used Hook in React Three is UseFrame, this one will take a function that will be called at each frame of your scene. Here is a link to learn how to use it:<br><br>
https://docs.pmnd.rs/react-three-fiber/api/hooks#useframe
<br>
```js
import { useFrame } from '@react-three/fiber'

function Foo() {
  useFrame((state, delta, xrFrame) => {
    // This function runs at the native refresh rate inside of a shared render-loop
})
```

<h2>Step 5:</h2><br>
Other materials are also widely used to make your sites unique and dynamic. Here, I'd like to introduce you to mesh portal material.<br>
Here's an example:<br>
https://r3-f-portal.vercel.app/ <br>
I suggest that you try to remake the same scene for this 5th step.

<h2>Step 6:</h2><br>
Enjoy ! If you liked this workshop, don't hesitate to star the repository :) !
<a href="https://github.com/RayanBn/React-Three-Js-Workshop2">Workshop 2</a>
