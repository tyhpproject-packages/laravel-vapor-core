<!-- tyhp-readme:start -->
# tyhpdef/laravel-vapor-core

Tyhp type definitions for `laravel/vapor-core` `2.47.0`.

```bash
composer require --dev tyhpdef/laravel-vapor-core:2.47.0
```

This is a metapackage. Composer also installs `tyhpdef/laravel-vapor-core-impl` (type files).
Require **this** name, not `tyhpdef/laravel-vapor-core-impl`.

See https://tyhplang.com.

## Maintain `laravel/vapor-core`? Ship the types yourself

If you are a Packagist maintainer of `laravel/vapor-core`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-vapor-core-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/vapor-core` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-vapor-core": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/vapor-core` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/vapor-core` with a real constraint,
   `"replace": { "tyhpdef/laravel-vapor-core": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/vapor-core` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-vapor-core` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
