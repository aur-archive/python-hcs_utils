# Maintainer: Scott Hansen (firecat53) firecat4153 at gmail
pkgname=python-hcs_utils
pkgver=1.1.1
pkgrel=2
pkgdesc="Collection of snippets that are used in multiple projects, primarily goobook"
arch=('any')
url="http://gitorious.org/hcs_utils"
license=('GPL')
provides=('hcs_utils')
depends=('python2')
makedepends=('python2-distribute')
source=("http://pypi.python.org/packages/source/h/hcs_utils/hcs_utils-1.1.1.tar.gz")
md5sums=('1add7548e0cf423b363fdd4e2ccafbd5')

build() {
  cd ${srcdir}/"hcs_utils-$pkgver"
  python2 setup.py build || return 1
  python2 setup.py install --root=${pkgdir} --optimize=1 || return 1
}
