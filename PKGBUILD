# Contributor: Tim Yang <tdy@gmx.com>
# Contributor: Christoph Siegenthaler <csi@gmx.ch>
pkgname=jp2a
pkgver=1.0.6
pkgrel=3
pkgdesc="A small utility for converting JPG images to ASCII"
arch=('i686' 'x86_64')
url="http://jp2a.sourceforge.net/"
license=('GPL')
depends=('curl' 'libjpeg')
source=(http://downloads.sourceforge.net/jp2a/jp2a-$pkgver.tar.gz)
md5sums=('eb6281eee29acf1c494dcaf7d745a5df')

build(){
  cd "$srcdir/jp2a-$pkgver"
  ./configure --prefix=/usr
  make
}

package(){
  cd "$srcdir/jp2a-$pkgver"
  make DESTDIR="$pkgdir" install
}
