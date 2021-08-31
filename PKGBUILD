pkgname=twitch-downloader
pkgver=3.0
pkgrel=1
pkgdesc="Easily download twitch VODs and Clips."
arch=('x86_64')
url="https://github.com/jybp/twitch-downloader"
license=('custom')
source=("https://github.com/jybp/$pkgname/archive/refs/tags/v$pkgver.tar.gz")
source=("https://github.com/jybp/$pkgname/releases/download/v$pkgver/twitchdl_${pkgver}_Linux_x86_64")
md5sums=('8d1c4bcf293a351a904bdaa4414eae29')

package() {
    mkdir -p "${pkgdir}/usr/local/bin/"
    cp "${srcdir}/twitchdl_${pkgver}_Linux_x86_64" "${pkgdir}/usr/local/bin/${pkgname}"
    chmod 755 "${pkgdir}/usr/local/bin/${pkgname}"
}

