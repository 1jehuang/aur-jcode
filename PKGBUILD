# Maintainer: Jeremy Huang <jeremyhuang55555@gmail.com>
pkgname=jcode-bin
pkgver=0.72.0
pkgrel=1
pkgdesc="AI coding agent powered by Claude and ChatGPT"
arch=('x86_64')
url="https://github.com/1jehuang/jcode"
license=('MIT')
provides=('jcode')
conflicts=('jcode')
source=("https://github.com/1jehuang/jcode/releases/download/v0.72.0/jcode-linux-x86_64.tar.gz")
sha256sums=('60fcbfab6c92e63e32d8a7ff757b5696479b338de455e4eb17180cfc927743ed')

package() {
    install -Dm755 "${srcdir}/jcode-linux-x86_64" "${pkgdir}/usr/lib/jcode/jcode-linux-x86_64"
    install -Dm755 "${srcdir}/jcode-linux-x86_64.bin" "${pkgdir}/usr/lib/jcode/jcode-linux-x86_64.bin"
    mkdir -p "${pkgdir}/usr/bin"
    ln -s /usr/lib/jcode/jcode-linux-x86_64 "${pkgdir}/usr/bin/jcode"
}
