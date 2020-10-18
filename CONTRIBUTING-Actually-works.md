This repo (and pbiviz) seem to rely on running on old versions of Node. It took quite a bit of sleuthing to work out exactly what the issue was.

# Switch to older versions of Node and NPM

nvm install 12.16.1
nvm use 12.16.1
nvm install-latest-npm

This gives you node 6.14.8 as well.

/Users/[user]/.nvm/versions/node/v12.16.1/

# Setup mapboxgl-powerbi

npm install -g powerbi-visuals-tools@2.6.0
pbiviz --create-cert
pbiviz --install-cert

npm install

npm install browserify eslint --save-dev

npm run turf-build

pbiviz update 1.13.0

pbiviz start

# Useful links

https://github.com/mapbox/mapboxgl-powerbi/issues/379
https://github.com/mapbox/mapboxgl-powerbi/issues/373
https://github.com/mapbox/mapboxgl-powerbi/issues/347
https://github.com/microsoft/PowerBI-visuals/issues/436
