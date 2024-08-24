# Maintainer: Quentin Bouvet <qbouvet at outlook dot com>
pkgname=bash-timer
pkgver=1.5.0
pkgrel=1
pkgdesc="Human-readable execution time for every command in bash!"
arch=('any')
url="https://github.com/hopeseekr/bash-timer"
license=('APACHE')
depends=('bash-preexec')

source=("${pkgname}-${pkgver}::https://github.com/hopeseekr/bash-timer/archive/v${pkgver}.tar.gz")
install=${pkgname}.install
sha256sums=('577be5bd1a5dd8818883cba4f840362a30e64c0440fb3647d784203f59eb37d8')

package() {
  cd "${srcdir}/"
  install -D -m0755 -t "${pkgdir}/usr/share/${pkgname}" \
    "${pkgname}-${pkgver}/${pkgname}.sh"
}

#
# makepkg --printsrcinfo > .SRCINFO
#
