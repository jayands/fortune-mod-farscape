# Maintainer: Daniel Woffinden <d.woffinden@live.co.uk>

pkgname=fortune-mod-farscape
pkgver=1
pkgrel=1
pkgdesc="farscape fortune cookie file"
arch=('any')
#url=""
license=('CC-BY-SA')
makedepends=('perl' 'perl-mediawiki-api' 'perl-libwww')
depends=('fortune-mod')
groups=('fortune-mods')
source=('wiki.pl')
md5sums=('f933fda52f1f33972254c7b570fd0cd1')

build() {
  cd ${srcdir}

  perl wiki.pl > farscape

  strfile farscape farscape.dat

  install -D -m644 farscape ${pkgdir}/usr/share/fortune/farscape
  install -D -m644 farscape.dat ${pkgdir}/usr/share/fortune/farscape.dat
}

