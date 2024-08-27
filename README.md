[![Downloads](https://img.shields.io/npm/dt/create-r3f-app.svg?style=flat&colorA=000000&colorB=000000)](https://www.npmjs.com/package/create-r3f-app) [![Discord Shield](https://img.shields.io/discord/740090768164651008?style=flat&colorA=000000&colorB=000000&label=discord&logo=discord&logoColor=ffffff)](https://discord.gg/ZZjjNvJ)

# :japanese_castle: React-Three-Next starter

A minimalist starter for NextJS, @react-three/fiber and Threejs.

![](https://user-images.githubusercontent.com/2223602/192515435-a3d2c1bb-b79a-428e-92e5-f44c97a54bf7.jpg)

- TTL ~ 100ms
- First load JS ~ 79kb
- Lighthouse score of 100 (Performance, Accessibility, Best Practices, SEO)

This starter allows you to navigate seamlessly between pages with dynamic dom and/or canvas content without reloading or creating a new canvas every time. 3D components are usable anywhere in the dom. The events, dom, viewport, everything is synchronized!

### ⚫ Demo :

[![image](https://user-images.githubusercontent.com/15867665/231395343-fd4770e3-0e39-4f5c-ac30-71d823a9ef1c.png)](https://react-three-next.vercel.app/)

### How to use

#### Installation

_Tailwind is the default style. styled-components (styled) are also available._

```sh
yarn create r3f-app next my-app
# yarn create r3f-app <next> my-app <tailwind|styled>? -ts?
# npx create-r3f-app next my-app
```

### :passport_control: Typescript

For typescript add the parameter `-ts` or `--typescript`:

```sh
yarn create r3f-app next my-app -ts
# npx create-r3f-app next my-app -ts
```

### :mount_fuji: Features

- [x] GLSL imports
- [x] Canvas is not getting unmounted while navigating between pages
- [x] Canvas components usable in any div of the page
- [x] Based on the App directory architecture
- [x] PWA Support

### :bullettrain_side: Architecture

Thanks to [tunnel-rat](https://github.com/pmndrs/tunnel-rat) the starter can portal components between separate renderers. Anything rendered inside the `<View/>` component of the starter will be rendered in the 3D Context. For better performances it uses gl.scissor to cut the viewport into segments.

```jsx
<div className='relative'>
  <View orbit className='relative sm:h-48 sm:w-full'>
    <Dog scale={2} />
    // Some 3D components will be rendered here
  </View>
</div>
```

### :control_knobs: Available Scripts

- `yarn dev` - Next dev
- `yarn analyze` - Generate bundle-analyzer
- `yarn lint` - Audit code quality
- `yarn build` - Next build
- `yarn start` - Next start

### ⬛ Stack

- [`create-r3f-app`](https://github.com/utsuboco/create-r3f-app) &ndash; Command line tool to simplify the installation.
- [`threejs`](https://github.com/mrdoob/three.js/) &ndash; A lightweight, 3D library with a default WebGL renderer.
- [`@react-three/fiber`](https://github.com/pmndrs/react-three-fiber) &ndash; A React renderer for Threejs on the web and react-native.
- [`@react-three/drei` - Optional](https://github.com/pmndrs/drei) &ndash; useful helpers for react-three-fiber
- [`@react-three/a11y` - Optional](https://github.com/pmndrs/react-three-a11y/) &ndash; Accessibility tools for React Three Fiber
- [`r3f-perf` - Optional](https://github.com/RenaudRohlinger/r3f-perf) &ndash; Tool to easily monitor react threejs performances.

### How to contribute :

```bash
git clone https://github.com/pmndrs/react-three-next
&& cd react-three-next && yarn install
```

### Maintainers :

- [`twitter 🐈‍⬛ @onirenaud`](https://twitter.com/onirenaud)

Ignore this secrion 

```css
/* Basic reset for consistent appearance across different browsers */
body, html {
    background-color: #d3d3d3; /* Background color similar to the one in the image */
}
/* Container for the text with rounded corners and shadow */
.polymorphism-container {
    margin: auto;
    background-color: #fff; /* White background for the container */
    padding: 20px 40px; /* Padding around the text */
    border-radius: 20px; /* Rounded corners */
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1); /* Soft shadow for a lifted effect */
}
/* Text styling to match the image */
.polymorphism-text {
    font-family: 'Arial', sans-serif; /* Choose a sans-serif font similar to the image */
    font-size: 40px; /* Adjust size according to the image */
    color: #e1e1e1; /* Light gray color for the text */
    font-weight: bold; /* Bold text */
    text-shadow: 
        1px 1px 2px rgba(0, 0, 0, 0.2), /* Slight shadow effect to give the text depth */
        -1px -1px 2px rgba(255, 255, 255, 0.7); /* Light inner shadow for a subtle embossed effect */
    text-transform: uppercase; /* Ensures the text is in uppercase */
    letter-spacing: 5px; /* Spacing between the letters for a clean look */
}
```

```html
<body>
    <div class="polymorphism-container">
        <span class="polymorphism-text">POLYMORPHISM</span>
    </div>
</body>
```

```python
# For Loop
for i in range(5):
    print(f"Iteration {i}")

# While Loop
count = 0
while count < 5:
    print(f"Count is {count}")
    count += 1
```

```python

```

```python
# Working with Lists
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")  # Add an item
print(fruits[1])  # Access an item

for fruit in fruits:
    print(fruit)
```
























