<<<<<<< 22050b01eef5db439e90b586284647615b93f885
# Maintainier: FadeMind <fademind@gmail.com>

pkgname=kdeartwork-wallpapers-archlinux-caledonia
_basename=archlinux-caledonia
pkgver=1.0
pkgrel=1
pkgdesc="Arch Linux Caledonia Wallpaper"
arch=('any')
license=('CCPL')
url="http://malisremac.deviantart.com/art/Arch-Linux-Caledonia-311824516"
depends=('kdebase-workspace')
optdepends=('caledonia-bundle: A bundle with all Caledonia customizations')
source=($_basename.zip::'https://copy.com/FD9JKQwErBknZQkY%2FArch+Linux+Caledonia.zip?download=1')
sha256sums=('ff749678ee022a8bcdb9f2ad10153f492d23e9eb06137f037120ede5d2ceb0a3')

package() {
	cd "$srcdir"
	find Arch\ Linux\ Caledonia/* -type f -exec install -Dm 644 '{}' "$pkgdir/usr/share/wallpapers/{}" \;
}
=======
# Maintainer: nosada <ngsksdt@gmail.com>
# Contributor: FadeMind <fademind@gmail.com>
# Contributor: sarkasper <echo a2FzcGVyLm1lbnRlbkBnbXguY29tCg==|base64 -d>

pkgname=caledonia-backgrounds
_pkgname=Caledonia_Official_Wallpaper_Collection
pkgver=2.0
pkgrel=1
pkgdesc="The official wallpaper collection for Caledonia (DE-independent)"
arch=('any')
url="http://malcer.deviantart.com"
license=('CCPL')
source=("http://sourceforge.net/projects/caledonia/files/Caledonia%20Official%20Wallpapers/Caledonia_Official_Wallpaper_Collection-${pkgver}.tar.gz")
sha256sums=('9488e00637af5ac10eddcea37063ac63d1b33010fbb5d4dae0060954001da917')

package() {
  cd ${srcdir}/${_pkgname}
  mkdir -p -m755 "${pkgdir}/usr/share/wallpapers/caledonia"
  rm README
  cp -rf --no-preserve=mode * "$pkgdir/usr/share/wallpapers/caledonia"
}
sha256sums=('42caaeff55359bb5789f2c624595a4d67011024ec5201d40212f381b82535e29')

# vim:set ts=2 sw=2 et:
>>>>>>> initial import
