Maintainer: Martin Wilson <martin at pipegrep dot co dot uk> 
pkgname=tarquin
pkgver=4.3.12
pkgrel=1
pkgdesc="An analysis tool for automatically determining the quantities of molecules present in MR spectroscopy data"
arch=("x86_64")
url="http://tarquin.sourceforge.net/"
license=('GPL')
#groups=()
depends=("gcc-fortran" "lapack" "protobuf" "qt4" "boost" "fftw" "protobuf" "gnuplot" "qwt5")
makedepends=("cmake")
#optdepends=()
#provides=()
#conflicts=()
#replaces=()
#backup=()
#options=()
#install=
#changelog=
source=(https://github.com/martin3141/tarquin/archive/v$pkgver.tar.gz)
#noextract=()
md5sums=() #autofill using updpkgsums

prepare() {

}

build() {
  cd "$pkgname-$pkgver"

  ./configure --prefix=/usr
  make
}

package() {
  cd "$pkgname-$pkgver"

  make DESTDIR="$pkgdir/" install
}
