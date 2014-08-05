Npm2Arch
========

Convert npm packages into a PKGBUILD for Archlinux integration.

NPM package.json --> PKGBUILD for pacman


Install
-------
### From AUR :
yaourt -S [nodejs-npm2arch](https://aur.archlinux.org/packages/nodejs-npm2arch/)


### From sources

    git clone https://github.com/Filirom1/npm2arch
    cd npm2arch
    [sudo] npm install -g


Usage
-----

### npm2PKGBUILD

Transform a npm package into an ArchLinux PKGBUILD

    npm2PKGBUILD `npm-name` > PKGBUILD
    makepkg
    pacman -U nodejs-`name`-`version`-any.pkg.tar.xz


### npm2archpkg

Transform a npm package into an ArchLinux package archive

    npm2archpkg `npm-name`
    pacman -U nodejs-`name`-`version`-any.pkg.tar.xz


### npm2archinstall

Install a npm package with pacman

    npm2archinstall `npm-name`


License
-------

npm2arch is licensed under the [MIT License](https://github.com/Filirom1/npm2arch/blob/master/LICENSE).
