# Is My Internet Working?

Official source code for the website [Is My Internet Working?](https://ismyinternetworking.com/). Now powered by Node.js.

**Looking for an offline version?** [Download a standalone version of IMIW](https://github.com/theBrianCui/IsMyInternetWorking/files/1786104/index.zip) that you can open locally and use offline.

## First Time Setup

Create a `.env` file in the base directory with the following:

```
NODE_ENV=production|dev
NODE_INLINE=true|false
```

The `production` build enables minifaction, Google Analytics, and other small changes. The `dev` build is faster and better suited for development purposes.

Install dependencies:

```
npm install
```

For location services, `freegeoip` must be running in the background listening on port 8080. Binaries are available for all [operating systems here.](https://github.com/fiorix/freegeoip/releases)

To build the project, run

```
npm run build
```

This will build project files in the `/build` directory.

To build the project AND start a local web server, run

```
npm run start
```

The site will be hosted at `localhost:8000`.
