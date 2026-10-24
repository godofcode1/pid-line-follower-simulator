# PID Line Follower Simulator

A static browser simulator for PID tuning and neural network training. The page includes eight selectable circuits, a 3D robot view, orbit/zoom controls, live sensor feedback, PID presets, and a small neural controller trained in the browser. A separate reference viewer loads the UKMARSBOT 3D model through Google's model-viewer web component.

## Run locally

Open `index.html` in a modern browser with an internet connection. Three.js is loaded from jsDelivr.

## Deploy

The `outputs` folder is ready to publish as a static site:

- **Vercel:** import the GitHub repository and use the default static settings. `vercel.json` is included.
- **Netlify:** import the GitHub repository and leave the build command blank. Set the publish directory to `outputs` if importing the parent repository, or `.` if importing this folder. `netlify.toml` is included.

## Robot design reference

The simulated robot is assembled from original geometric parts in the page. The physical design reference is [UKMARSBOT](https://github.com/ukmars/ukmarsbot), an open-source two-wheel robotics platform released under the MIT license. Its separately licensed preview model is served by [Robotheca](https://robotheca.org/robots/ukmarsbot) and is loaded only when the model viewer is opened.
