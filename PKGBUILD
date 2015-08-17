# Maintainer: evr <evanroman @ gmail>

pkgname=tpfand-profiles
pkgver=20120603
pkgrel=2
pkgdesc="tpfand profiles for various IBM/Lenovo Thinkpad models"
arch=('any')
url="http://www.gambitchess.org/mediawiki/index.php/ThinkPad_Fan_Control"
license=('GPL3')
depends=(tpfand)
optdepends=(tpfan-admin)
source=(http://tpfanco.googlecode.com/files/${pkgname}_${pkgver}_all.deb)

package() {
  cd "$srcdir"
  ar x ${pkgname}_${pkgver}_all.deb
  tar xf data.tar.gz
  install -d "$pkgdir"/usr/share/tpfand/models/{by-id,by-name} 
  install -m644 "$srcdir"/usr/share/tpfand/models/by-id/* "$pkgdir"/usr/share/tpfand/models/by-id/ 
}

md5sums=('3a962ccebcdcd47ddd83d2202dc2e1c2')
sha1sums=('5bdb777cc3da9e0d8b76cec80aa0d68e0582a19f')
