# Getting started


A config has been added to `packages/test-package/package.json` but it doesn't work. 

You can check it out by running:

```shell
yarn
yarn build
```

Then try to add the following config to `/package.json` (workspace root):

```json
  "@parcel/resolver-default": {
    "packageExports": true
  }
```

Run the following command afterwards:

```shell
yarn clean  # to clean parcel caches.
yarn build
```

It will work and applies the config correctly.

[Github issue](https://github.com/parcel-bundler/parcel/issues/9602)
