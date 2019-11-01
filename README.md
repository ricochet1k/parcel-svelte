This repo is currently being used to report bugs in Parcel 2 and develop parcel-transformer-svelte

This repo is setup to use Yalc to include the in-development version of parcel 2 checkout from git.

Yalc publish all in the parcel repository:
```sh
for p in packages/*/package.json packages/*/*/packages.json; do ( cd $(dirname $p); yalc push ) ; done
```

Then run with
```sh
yalc update
yarn
yarn run parcel
```

