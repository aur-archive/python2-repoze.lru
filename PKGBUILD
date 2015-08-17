# Maintainer : DasIch <dasdasich@googlemail.com>
# Contributor: James Bulmer <nekinie@gmail.com>

pkgname="python2-repoze.lru"
pkgver=0.6
pkgrel=2
pkgdesc="A tiny LRU cache implementation and decorator"
arch=("any")
url="https://pypi.python.org/pypi/repoze.lru"
license=("custom:BSD")
depends=("python2")
makedepends=("python2-setuptools")
source=("https://pypi.python.org/packages/source/r/repoze.lru/repoze.lru-${pkgver}.tar.gz")
md5sums=("2c3b64b17a8e18b405f55d46173e14dd")

build() {
    cd "${srcdir}/repoze.lru-${pkgver}/"
    python2 setup.py build
}

package() {
  cd "${srcdir}/repoze.lru-${pkgver}/"
  python2 setup.py install --root="${pkgdir}/" --optimize=1
}
