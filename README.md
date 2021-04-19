# {projectName}

- {description}

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run lint`

Runs linter of ESLint and TSC, that will prevent bugs!

### `npm run coverage`

Launches the test runner and display to coverage.\
That find the test coverage rate.\
> Note: That it is not very accurate, At least Hook and JSX coverage is incomplete.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Available Enviroment variables

You can adjust various development and production settings by setting environment variables in your shell or with .env.

> Note: You do not need to declare `REACT_APP_` before the below variables as you would with custom environment variables.

| Variable                  | Development | Production | Usage                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| :------------------------ | :---------: | :--------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BROWSER                   |   ✅ Used   | 🚫 Ignored | By default, Create React App will open the default system browser, favoring Chrome on macOS. Specify a [browser](https://github.com/sindresorhus/open#app) to override this behavior, or set it to `none` to disable it completely. If you need to customize the way the browser is launched, you can specify a node script instead. Any arguments passed to `npm start` will also be passed to this script, and the url where your app is served will be the last argument. Your script's file name must have the `.js` extension.                                                                                                                                      |
| BROWSER_ARGS              |   ✅ Used   | 🚫 Ignored | When the `BROWSER` environment variable is specified, any arguments that you set to this environment variable will be passed to the browser instance. Multiple arguments are supported as a space separated list. By default, no arguments are passed through to browsers.                                                                                                                                                                                                                                                                                                                                                                                               |
| HOST                      |   ✅ Used   | 🚫 Ignored | By default, the development web server binds to all hostnames on the device (`localhost`, LAN network address, etc.). You may use this variable to specify a different host.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| PORT                      |   ✅ Used   | 🚫 Ignored | By default, the development web server will attempt to listen on port 3000 or prompt you to attempt the next available port. You may use this variable to specify a different port.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| HTTPS                     |   ✅ Used   | 🚫 Ignored | When set to `true`, Create React App will run the development server in `https` mode.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| WDS_SOCKET_HOST           |   ✅ Used   | 🚫 Ignored | When set, Create React App will run the development server with a custom websocket hostname for hot module reloading. Normally, `webpack-dev-server` defaults to `window.location.hostname` for the SockJS hostname. You may use this variable to start local development on more than one Create React App project at a time. See [webpack-dev-server documentation](https://webpack.js.org/configuration/dev-server/#devserversockhost) for more details.                                                                                                                                                                                                              |
| WDS_SOCKET_PATH           |   ✅ Used   | 🚫 Ignored | When set, Create React App will run the development server with a custom websocket path for hot module reloading. Normally, `webpack-dev-server` defaults to `/sockjs-node` for the SockJS pathname. You may use this variable to start local development on more than one Create React App project at a time. See [webpack-dev-server documentation](https://webpack.js.org/configuration/dev-server/#devserversockpath) for more details.                                                                                                                                                                                                                              |
| WDS_SOCKET_PORT           |   ✅ Used   | 🚫 Ignored | When set, Create React App will run the development server with a custom websocket port for hot module reloading. Normally, `webpack-dev-server` defaults to `window.location.port` for the SockJS port. You may use this variable to start local development on more than one Create React App project at a time. See [webpack-dev-server documentation](https://webpack.js.org/configuration/dev-server/#devserversockport) for more details.                                                                                                                                                                                                                          |
| PUBLIC_URL                |   ✅ Used   |  ✅ Used   | Create React App assumes your application is hosted at the serving web server's root or a subpath as specified in [`package.json` (`homepage`)](deployment#building-for-relative-paths). Normally, Create React App ignores the hostname. You may use this variable to force assets to be referenced verbatim to the url you provide (hostname included). This may be particularly useful when using a CDN to host your application.                                                                                                                                                                                                                                     |
| BUILD_PATH                | 🚫 Ignored  |  ✅ Used   | By default, Create React App will output compiled assets to a `/build` directory adjacent to your `/src`. You may use this variable to specify a new path for Create React App to output assets. BUILD_PATH should be specified as a path relative to the root of your project.                                                                                                                                                                                                                                                                                                                                                                                          |
| CI                        |   ✅ Used   |  ✅ Used   | When set to `true`, Create React App treats warnings as failures in the build. It also makes the test runner non-watching. Most CIs set this flag by default.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| REACT_EDITOR              |   ✅ Used   | 🚫 Ignored | When an app crashes in development, you will see an error overlay with clickable stack trace. When you click on it, Create React App will try to determine the editor you are using based on currently running processes, and open the relevant source file. You can [send a pull request to detect your editor of choice](https://github.com/facebook/create-react-app/issues/2636). Setting this environment variable overrides the automatic detection. If you do it, make sure your systems [PATH](<https://en.wikipedia.org/wiki/PATH_(variable)>) environment variable points to your editor’s bin folder. You can also set it to `none` to disable it completely. |
| CHOKIDAR_USEPOLLING       |   ✅ Used   | 🚫 Ignored | When set to `true`, the watcher runs in polling mode, as necessary inside a VM. Use this option if `npm start` isn't detecting changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| GENERATE_SOURCEMAP        | 🚫 Ignored  |  ✅ Used   | When set to `false`, source maps are not generated for a production build. This solves out of memory (OOM) issues on some smaller machines.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| INLINE_RUNTIME_CHUNK      | 🚫 Ignored  |  ✅ Used   | By default, Create React App will embed the runtime script into `index.html` during the production build. When set to `false`, the script will not be embedded and will be imported as usual. This is normally required when dealing with CSP.                                                                                                                                                                                                                                                                                                                                                                                                                           |
| IMAGE_INLINE_SIZE_LIMIT   |   ✅ Used   |  ✅ Used   | By default, images smaller than 10,000 bytes are encoded as a data URI in base64 and inlined in the CSS or JS build artifact. Set this to control the size limit in bytes. Setting it to `0` will disable the inlining of images.                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| FAST_REFRESH              |   ✅ Used   | 🚫 Ignored | When set to `false`, disables experimental support for Fast Refresh to allow you to tweak your components in real time without reloading the page.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| TSC_COMPILE_ON_ERROR      |   ✅ Used   |  ✅ Used   | When set to `true`, you can run and properly build TypeScript projects even if there are TypeScript type check errors. These errors are printed as warnings in the terminal and/or browser console.                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ESLINT_NO_DEV_ERRORS      |   ✅ Used   | 🚫 Ignored | When set to `true`, ESLint errors are converted to warnings during development. As a result, ESLint output will no longer appear in the error overlay.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| DISABLE_ESLINT_PLUGIN     |   ✅ Used   |  ✅ Used   | When set to `true`, [eslint-webpack-plugin](https://github.com/webpack-contrib/eslint-webpack-plugin) will be completely disabled.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| DISABLE_NEW_JSX_TRANSFORM |   ✅ Used   |  ✅ Used   | When set to `true`, disables the [new JSX transform](https://reactjs.org/blog/2020/09/22/introducing-the-new-jsx-transform.html) introduced in React 17 and backported to React 16.14.0, 15.7.0, and 0.14.10. New projects will use a version of React that supports this by default but you may need to disable it in existing projects if you can't upgrade React.                                                                                                                                                                                                                                                                                                     |

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
