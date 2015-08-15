# Maintainer: Filip Graliński <filipg@amu.edu.pl>
pkgname=giza-pp
pkgver=1.0.7
pkgrel=3
pkgdesc='A statical machine translation toolkit used to train word alignment models'
arch=('i686' 'x86_64')
url='https://code.google.com/p/giza-pp/'
license=('GPL2')
makedepends=(gcc make)
depends=(tcsh gcc-libs)
install=
source=(https://giza-pp.googlecode.com/files/giza-pp-v1.0.7.tar.gz)
md5sums=('bbc15f8add7def89768c6e253c91a65d')

build() {
  cd "${srcdir}/${pkgname}"

  make
}

package() {
  cd "${srcdir}/${pkgname}"

  install -D "GIZA++-v2/GIZA++" "${pkgdir}/usr/bin/GIZA++"
  install -D "GIZA++-v2/plain2snt.out" "${pkgdir}/usr/bin/plain2snt.out"
  install -D "GIZA++-v2/snt2cooc.out" "${pkgdir}/usr/bin/snt2cooc.out"
  install -D "GIZA++-v2/trainGIZA++.sh" "${pkgdir}/usr/bin/trainGIZA++.sh"
  install -D "mkcls-v2/mkcls" "${pkgdir}/usr/bin/mkcls"
}
