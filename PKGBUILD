# Maintainer: ponsfoot <cabezon dot hashimoto at gmail dot com>

pkgname=ttf-umeplus-cl
pkgver=20140427
pkgrel=1
pkgdesc="Japanese TrueType gothic fonts, based on Ume Gothic CL and M+ Fonts"
url="http://www.geocities.jp/ep3797/modified_fonts_01.html"
license=('custom')
arch=('any')
depends=('fontconfig' 'xorg-font-utils')
install=ttf.install
source=(http://downloads.sourceforge.net/mdk-ut/umeplus-cl-fonts-${pkgver}.tar.lzma)
md5sums=('c677952f1e177c920ae560b92ca79f2c')

package() {
  cd "${srcdir}/umeplus-cl-fonts-${pkgver}"

  install -d "${pkgdir}/usr/share/fonts/TTF"
  install -m644 *.ttf "${pkgdir}/usr/share/fonts/TTF"

  install -D -m644 docs-mplus/LICENSE_E \
          "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE-MPLUS.txt"
  install    -m644 docs-ume/license.html \
          "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE-UME.html"
}
