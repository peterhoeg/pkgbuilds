# Maintainer: Peter Hoeg <first name at last name dot com>
# Contributor: FadeMind <fademind@gmail.com>
# Contributor: Tommaso Sardelli <lacapannadelloziotom [at] gmail [dot] com>
# Contributor: nosada <ngsksdt@gmail.com>
# Contributor: sarkasper <echo a2FzcGVyLm1lbnRlbkBnbXguY29tCg==|base64 -d>

pkgname=caledonia-backgrounds
pkgver=2.0
pkgrel=2
pkgdesc='Caledonia theme: DE-independent wallpapers/backgrounds'
arch=('any')
url=('http://caledonia.sourceforge.net')
license=('CCPL:by-sa')
conflicts=('caledonia-bundle' 'caledonia-bundle-plasma5')
replaces=()
source=("http://sourceforge.net/projects/caledonia/files/Caledonia%20Official%20Wallpapers/Caledonia_Official_Wallpaper_Collection-${pkgver}.tar.gz")
sha256sums=('42caaeff55359bb5789f2c624595a4d67011024ec5201d40212f381b82535e29')

package() {
  mkdir -p -m755 \
        "${pkgdir}/usr/share/wallpapers" \
        "${pkgdir}/usr/share/doc/${pkgname}"

  mv Caledonia_Official_Wallpaper_Collection/README "${pkgdir}/usr/share/doc/${pkgname}"
  cp -r Caledonia_Official_Wallpaper_Collection/* "${pkgdir}/usr/share/wallpapers"

  find "$pkgdir" -type d -print0 | xargs -0 chmod 755
  find "$pkgdir" -type f -print0 | xargs -0 chmod 644
}
