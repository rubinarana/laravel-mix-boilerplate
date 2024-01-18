## Introduction
Boilerplate for fresh Html project which support hot-reload. 
Supports SCSS.

## Installation
1.  Clone the repository
2.  Install dependencies:
    npm ci (Installing dependencies exactly as specified in the package-lock.json file.)
3.  Build assets using Laravel Mix:
    npm run mix
    For more info:
    https://laravel-mix.com/docs/6.0/installation
4.  For Hot reload
    npm run watch

## Folder Structure
1. /assets: contain overall fonts, image, script and styles.
2. /dist: Compiled assets's files.

## Dependencies
Bootstrap 5
SCSS
Laravel Mix
Live Server

## live server for hot reload.
var params = {
	port: 8181, // Set the server port. Defaults to 8080.
	host: "0.0.0.0", // Set the address to bind to. Defaults to 0.0.0.0 or process.env.IP.
	open: false, // When false, it won't load your browser by default.
	ignore: 'assets,my/templates', // comma-separated string for paths to ignore
	file: "index.html", // When set, serve this file (server root relative) for every 404 (useful for single-page applications)
	wait: 1000, // Waits for all changes, before reloading. Defaults to 0 sec.
	mount: [['/components', './node_modules']], // Mount a directory to a route.
	logLevel: 2, // 0 = errors only, 1 = some, 2 = lots
	middleware: [function(req, res, next) { next(); }] // Takes an array of Connect-compatible middleware that are injected into the server middleware stack
};
https://www.npmjs.com/package/live-server

## Pages Path
For index page :http://localhost:8181/index.html