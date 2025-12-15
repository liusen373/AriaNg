# AriaNg

## Introduction
AriaNg is a modern web frontend making [aria2](https://github.com/aria2/aria2) easier to use. AriaNg is written in pure html & javascript, thus it does not need any compilers or runtime environment. You can just put AriaNg in your web server and open it in your browser. AriaNg uses responsive layout, and supports any desktop or mobile devices.

This repository is a fork of AriaNg that removes unnecessary restrictions from the upstream version. Now you can manage your local aria2 daemon with an AriaNg instance hosted on *any* server.

- **You don't have to** enable HTTPS for a locally used aria2 and maintain a TLS certificate that requires monthly renewal.
- **You don't have to** download a bloated Electron app (yet another Chrome browser), which is hundreds of times larger, consumes thousands of times more memory, and launches dozens of times slower than aria2 itself.

## Installation
AriaNg now provides three versions, standard version, all-in-one version and [AriaNg Native](https://github.com/mayswind/AriaNg-Native). Standard version is suitable for deployment in the web server, and provides on-demand loading. All-In-One version is suitable for local using, and you can download it and just open the only html file in browser. [AriaNg Native](https://github.com/mayswind/AriaNg-Native) is also suitable for local using, and is no need for browser. 

#### Prebuilt release

This repository syncs with the upstream daily and provides prebuilt release based on the latest commit (offering both standard version and all-in-one version). You can download them from [GitHub Actions](https://github.com/liusen373/AriaNg/actions/workflows/build.yml).

#### Building from source
Make sure you have [Node.js](https://nodejs.org/), [NPM](https://www.npmjs.com/) and [Gulp](https://gulpjs.com/) installed. Then download the source code, and follow these steps.

##### Standard Version

    $ npm install
    $ gulp clean build

##### All-In-One Version

    $ npm install
    $ gulp clean build-bundle

The builds will be placed in the dist directory.

## Demo
Please visit [http://ariang.mayswind.net/latest](http://ariang.mayswind.net/latest)

## License
[MIT](https://github.com/mayswind/AriaNg/blob/master/LICENSE)
