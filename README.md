# ipz

"ipz" stands for "install please".

It's a really dumb script for building newer (usually the bleeding edge
branches of) things on Debian-stable.

## Usage

 - clone this repo

 - put something like this in your shell rc:

```sh
for d in ~/.ipz/*; do
    export PATH=$d/bin:$PATH
done
```

 - run `./ipz <pkg>` where `<pkg>` is one of the files in the `pkgs` directory.
   E.g. `./ipz neovim`.

 - source your shell rc (or start a new shell) to get the new package in your
   path.


## Notes

 - To uninstall something, just delete `~/.ipz/<pkg>`
 - To upgrade something, uninstall the package and re-run the install.
