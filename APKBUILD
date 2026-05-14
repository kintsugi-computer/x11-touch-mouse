# Contributor: Kintsugi Computer <kintsugi.computer@protonmail.com>
# Maintainer: Kintsugi Computer <kintsugi.computer@protonmail.com>
pkgname=x11-touch-mouse
pkgver=1.1.1
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
dfa33f22cf58781241202019dee6e728d92553f398d8aba2084eb286cab2aa99961fb77ab44c29322ee6a7306d7cada48c896c066563f8343e08a0383fba0a7c  x11-touch-mouse-1.1.0.tar.gz
"
