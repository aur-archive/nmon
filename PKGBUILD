# Contributor: Massimiliano Torromeo <massimiliano.torromeo@gmail.com>

pkgname=nmon
pkgver=14g
pkgrel=1
pkgdesc="AIX & Linux Performance Monitoring tool"
arch=('i686' 'x86_64')
url="http://nmon.sourceforge.net"
license="GPL"
source=("http://downloads.sourceforge.net/${pkgname}/lmon$pkgver.c")

build() {
	cd ${srcdir}
	cc -o nmon lmon$pkgver.c -g -O2 -D JFS -D GETUSER -Wall -D LARGEMEM -lncurses -g
	install -D -m 0755 nmon "${pkgdir}/usr/bin/nmon"
}

md5sums=('e537f51446fb375140368b115dc8278b')
