# Maintainer: Anton Larionov <diffident dot cat at gmail dot com>

pkgname=yarxi
pkgver=1.10
pkgrel=2
pkgdesc="Japanese-Russian kanji dictionary"
arch=('i686' 'x86_64')
url="http://www.susi.ru/yarxi/mac_linux.html"
license=('unknown')
depends=('qt4')
install=${pkgname}.install

if [ "$CARCH" == "i686" ]; then
  source=("http://www.susi.ru/${pkgname}/${pkgname}_${pkgver}-1_i386.deb")
  md5sums=('6a294572c60b84f30513620e997c62da')
else
  source=("http://www.susi.ru/${pkgname}/${pkgname}_${pkgver}-1_amd64.deb")
  md5sums=('812d2265816ed781751c5c0eb6664d91')
fi

build() {
   cd "$srcdir"
   tar -zxvf data.tar.gz
}

package() {
  cd "$srcdir"
  cp -ra usr "$pkgdir/"
}

# vim:set ts=2 sw=2 et:
