This repository is based on [electron-quick-start](https://github.com/electron/electron-quick-start) repo and [spectron](https://github.com/electron-userland/spectron) repo.

I created this repo to be able to share the error Im seeing when using electron and spectron together.

The error Im getting is the following:

```
Application launch
    1) "before each" hook for "shows an initial window"


  0 passing (1s)
  1 failing

  1) Application launch
       "before each" hook for "shows an initial window":
     Error: Failed to create session.
unknown error: Chrome failed to start: exited abnormally.
  (unknown error: DevToolsActivePort file doesn't exist)
  (The process started from chrome location /Users/albertf/Test/electron-quick-start/node_modules/spectron/lib/launcher.js is no longer running, so ChromeDriver is assuming that Chrome has crashed.)
      at Object.startWebDriverSession (node_modules/webdriver/build/utils.js:34:15)
      at processTicksAndRejections (internal/process/task_queues.js:97:5)


```

With versions in used:

```
albertf@albertf-mac electron-quick-start % npm ls spectron electron                         
electron-quick-start@1.0.0 /Users/albertf/Test/electron-quick-start
├── electron@10.3.0 
└── spectron@12.0.0 
```

which are compatible versions according to [spectron](https://github.com/electron-userland/spectron#version-map)


# quickstart


```bash
# Go into the repository
nvm install
# Install dependencies
npm install
# Run the app
npm test
```

