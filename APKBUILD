# Contributor: Kintsugi Computer <kintsugi.computer@protonmail.com>
# Maintainer: Kintsugi Computer <kintsugi.computer@protonmail.com>
pkgname=x11-touch-mouse
pkgver=1.0.1
pkgrel=0
pkgdesc="Translate Kobo touchscreen events into X11 mouse events"
url="https://github.com/kintsugi-computer/x11-touch-mouse"
arch="armhf"
license="GPL2"
depends="xdotool"
makedepends="xdotool-dev"
source="https://github.com/kintsugi-computer/$pkgname/releases/download/v$pkgver/x11-touch-mouse-$pkgver.tar.gz"

builddir="$srcdir"/$pkgname-$pkgver

build () {
	./configure --prefix=/usr \
		--sysconfdir=/etc \
		--mandir=/usr/share/man \
		--infodir=/usr/share/info
	make
}

package () {
	make DESTDIR="$pkgdir" install
}

sha512sums="
1d9138dd65077c2d5823e5dfdf571a80d7363c09b6b128388d19ece3b75fcf38155a77d0e2f2dbfc4d3c3b58ec14df4e2e483c7c3b0335873f1b063eca00dfe6  x11-touch-mouse-1.0.1.tar.gz
"
