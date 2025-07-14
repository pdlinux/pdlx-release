# Maintainer: aliasadi <ali.asady@gmail.com>
pkgname=pdlx-release
pkgver=1.0
pkgrel=1
pkgdesc="Branding package for PdLinuXOS (os-release, lsb-release, issue, neofetch logo, pixmap, nushell config)"
arch=('any')
license=('GPL')
depends=('fastfetch' 'nushell')
source=(
    'os-release'
    'lsb-release'
    'issue'
    'pdlinuxos.txt'
    'pdlinuxos.png'
    'config.nu'
    '.bash_profile'
)
sha256sums=('SKIP' 'SKIP' 'SKIP' 'SKIP' 'SKIP' 'SKIP' 'SKIP')

package() {
    install -Dm644 "$srcdir/os-release" "$pkgdir/etc/os-release"
    install -Dm644 "$srcdir/lsb-release" "$pkgdir/etc/lsb-release"
    install -Dm644 "$srcdir/issue" "$pkgdir/etc/issue"
    install -Dm644 "$srcdir/pdlinuxos.txt" "$pkgdir/usr/share/neofetch/ascii/pdlinuxos.txt"
    install -Dm644 "$srcdir/pdlinuxos.png" "$pkgdir/usr/share/pixmaps/pdlinuxos.png"
    install -Dm644 "$srcdir/config.nu" "$pkgdir/etc/skel/.config/nushell/config.nu"
    install -Dm644 "$srcdir/.bash_profile" "$pkgdir/etc/skel/.bash_profile"
}
