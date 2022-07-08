<h1 alt="logo" align="center">Yaf - Yet Another Fetch</h1>
<div align="center">
<img src="https://i.imgur.com/nOceLGj.png" alt="yaf">
</div>

<br/>
<div align="center">
<a href="./LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge"></a>
<a href="https://github.com/deepjyoti30/yaf/releases"><img src="https://img.shields.io/github/v/release/deepjyoti30/yaf?style=for-the-badge"></a>
<img src="https://img.shields.io/badge/Built%20With-Golang-green?style=for-the-badge">

<br/>

### \[[Support](#support)] \[[Installation](#installation)] \[[Usage](#usage)]
<br/>
</div>


## Brief

Yet Another Fetch is a tool that fetches system information and shows it in a beautiful way for some extra upvotes on r/unixporn. It is extremely minimal and customizability is it's strong feature. Don't want to show your disk usage? Hide it with the `exclude` flag. Want to change the separator between the `os` and `Arch Linux` field? Use `separator` flag.

`yaf` is written in Golang. (Because everyone is writing a fetch in some language, why not Go then?)

## Installation

- [Binary](#binary)
- [Arch Linux](#arch-linux)
- [Gentoo Linux](#gentoo-linux)
- [Manual](#manual)

### Binary

Get the [latest release](https://github.com/deepjyoti30/yaf/releases) binary from GitHub and use it on your system. Yes, as simple as that.

### Arch Linux

`yaf` is available on [AUR here](https://aur.archlinux.org/packages/yafetch) and can be installed with:

```console
yay -S yafetch
```

or

```console
paru -S yafetch
```

>NOTE: `yaf` was taken so had to publish with `yafetch` name.

### Gentoo Linux

You can install yaf, by adding the overlay to layman with this command
```console
sudo layman -a thamognya
```
and then you can do 

```console
sudo emerge -a yaf
```
It will ask you to unmask it, as it is still testing for bugs (this is standard procedure for new ebuilds) hence you can unmask it by doing
```console
sudo emerge yaf --autounmask && dispatch-conf
``` 
then type `u` 

and then emerge it with the following command

```console
sudo emerge -a yaf --autounmask
```

and then install the package how you would normally.


### Manual

If you wish, you can install the package manually using the following:

- Clone the repo: `git clone git@github.com:deepjyoti30/yaf.git`
- Cd into the repo and use make to install the package: `cd yaf && make install`

> NOTE: You might want to use the mighty `sudo` with the make command above.

## Usage

```console
Usage of yaf:
  -exclude disk os
    	Exclude the passed fields from output. Values should be space separated, eg: disk os (default "username hostname")
  -key-prefix string
    	Prefix to be set before the key is printed (default "▪ ")
  -no-color
    	Disable showing colors in the output
  -separator string
    	Separator to be used between the key and the value (default "  ")
```

## Support

If you like this package and my [other works](https://github.com/deepjyoti30), your support would be appreciated!

<p align="left">
<a href="https://www.paypal.me/deepjyoti30" target="_blank"><img alt="undefined" src="https://img.shields.io/badge/paypal-deepjyoti30-blue?style=for-the-badge&logo=paypal"></a>
<a href="https://www.patreon.com/deepjyoti30" target="_blank"><img alt="undefined" src="https://img.shields.io/badge/Patreon-deepjyoti30-orange?style=for-the-badge&logo=patreon"></a>
<a href="https://ko-fi.com/deepjyoti30" target="_blank"><img alt="undefined" src="https://img.shields.io/badge/KoFi-deepjyoti30-red?style=for-the-badge&logo=ko-fi"></a>
</p>

## Contribution

Your contribution would be appreciated. Consider taking a look at the [guidelines](https://github.com/deepjyoti30/yaf/blob/master/.github/CONTRIBUTING.md) before opening a PR. If you just want a new feature added, you can open a feature request!
