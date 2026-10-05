<!-- tyhp-readme:start -->
# tyhpdef/psy-psysh

Tyhp type definitions for `psy/psysh` `0.12.24`.

```bash
composer require --dev tyhpdef/psy-psysh:0.12.24
```

This is a metapackage. Composer also installs `tyhpdef/psy-psysh-impl` (type files).
Require **this** name, not `tyhpdef/psy-psysh-impl`.

See https://tyhplang.com.

## Maintain `psy/psysh`? Ship the types yourself

If you are a Packagist maintainer of `psy/psysh`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/psy-psysh-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `psy/psysh` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/psy-psysh": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `psy/psysh` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `psy/psysh` with a real constraint,
   `"replace": { "tyhpdef/psy-psysh": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `psy/psysh` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/psy-psysh` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
