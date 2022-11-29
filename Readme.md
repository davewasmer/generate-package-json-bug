Reproduction repo for [nrwl/nx#13462](https://github.com/nrwl/nx/issues/13462)

The [type-only import in `myapp/src/main.ts`](./packages/myapp/src/main.ts) results in the dependencies of the [util package](./packages/utils/src/index.ts) (namely, `lodash`) being [included in the generated package.json file](./dist/packages/myapp/package.json#L5) produced by `generatePackageJson: true` while building myapp.
