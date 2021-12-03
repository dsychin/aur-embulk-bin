# Maintainer: Takuya Tominaga <takuya.tominaga.public at gmail dot com>

_pkgname=embulk
pkgname=$_pkgname-bin
pkgver=0.9.24
pkgrel=1
pkgdesc="Pluggable Bulk Data Loader."
arch=('i686' 'x86_64')
url="https://github.com/embulk/embulk"
license=('Apache')
depends=('jdk8-openjdk' 'nodejs')

_dl_url=https://github.com/embulk/embulk/releases/download
source_i686=("$_dl_url/v$pkgver/$_pkgname-$pkgver.jar"
)
source_x86_64=("$_dl_url/v$pkgver/$_pkgname-$pkgver.jar"
)
md5sums_i686=('SKIP'
)
md5sums_x86_64=('SKIP'
)



package() {
  _source_arch="32"
  [ "$CARCH" = "x86_64" ] && _source_arch="64"

  install -Dm755 "$srcdir/$_pkgname-$pkgver.jar" "$pkgdir/usr/bin/$_pkgname"
}

