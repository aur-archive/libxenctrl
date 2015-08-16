# Contributor: archtux
# Maintainer: ansgras <ataflinski@uni-koblenz.de>

pkgname=libxenctrl
pkgver=4.1.2
pkgrel=2
pkgdesc="Static libraries and header files for Xen"
arch=('i686' 'x86_64')
url="http://www.xen.org/"
license=('GPL')

if [ "${CARCH}" = 'x86_64' ]; then
  source=(http://mirrors.kernel.org/mandrake/Mandrakelinux/devel/cooker/x86_64/media/main/release/lib64xen-devel-$pkgver-1-mdv2012.0.x86_64.rpm)
  md5sums=('cc8f03ce613cdb98603567f3416b9eb0')
elif  [ "${CARCH}" = 'i686' ]; then 
  source=(http://mirrors.kernel.org/mandrake/Mandrakelinux/devel/cooker/i586/media/main/release/libxen-devel-$pkgver-1-mdv2012.0.i586.rpm)
  md5sums=('b87d4da1475f2ae49b2dac04df88b0eb')
fi

build() {
  cd $startdir

  bsdtar xf lib* -C $pkgdir
}
