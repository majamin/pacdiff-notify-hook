# Maintainer: Marian Minar <majamin _at_ gmail _dot_ com>
pkgname=pacdiff-notify-hook
pkgver=0.1.0
pkgrel=1
pkgdesc='Pacman hook that lists pending .pacnew files'
arch=('any')
url='https://github.com/majamin/pacdiff-notify-hook'
license=('MIT')
depends=('pacman-contrib')
conflicts=('pacdiff-pacman-hook-git')
source=('pacdiff-notify'
        'pacdiff-notify.hook')
sha256sums=('d3518fbaf8f603e515b79a032ea867336af521eeaf950a9b0a17277e7522530d'
            '6d806c3390fdfe692f9d4a1cfecd2adea77de39c3431c9ea250a53e836431abb')

package() {
    install -Dm755 pacdiff-notify \
        "$pkgdir/usr/share/libalpm/scripts/pacdiff-notify"
    install -Dm644 pacdiff-notify.hook \
        "$pkgdir/usr/share/libalpm/hooks/pacdiff-notify.hook"
}
