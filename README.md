# Pathfinding Visualizer
https://pathfinder-visualiser-870c6.web.app/ : link for you to have fun too!!
Welcome to Pathfinder Visualiser! This application explores two pathfinding algorithms, and visualises them as well. 

If you encounter any error or bugs Please reach out so that I could fix them! Thank you for trying out the project 

# Previous Issues
There were 2 issues recognised with the previous versions which have now been resolved:

1. When new obstacles were introduced into the grid after a computation the Dijkstra's algorithm specificallly was not able to retrieve the newer version of the grid and was still computing the results based on the previous Values. A* algorithms is updated with runtime so this issue was notfound there. This was ovrecome by calling The minorResetGrid function before calling Dijkstra funtion and updating all the states for the nodes(PathfinderVisualizer.jsx Line 311)

2. The grid is updated using methods such as onMouseUp, onMouseDown, onMouseEnter and onMouseLeave. This is used to simulate the mouse behaviour while interacting with the grid but the project can be used with a trackpad and touch screen as well which results in the grid not being updated after continued use(While using trackpad or touch screen). 

### Algorithms

This application supports the following algorithms:

- Dijkstra's Algorithm (weighted): the father of pathfinding algorithms; guarantees the shortest path

- A Search* (weighted): arguably the best pathfinding algorithm; uses heuristics to guarantee the shortest path much faster than Dijkstra's Algorithm

## Errors

For SAAS not found error run the command "npm install --save-dev node-sass sass-loader style-loader css-loader mini-css-extract-plugin --legacy-peer-deps" to make it work

for firbase init use "Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass"

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
