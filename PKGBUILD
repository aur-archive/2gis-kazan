pkgname=2gis-kazan
pkgver=54
pkgrel=2
pkgdesc="Map of Kazan for 2GIS, May 2013"
arch=('i686' 'x86_64')
url="http://kazan.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Kazan-54.orig.zip")
md5sums=('0282e9a05ed38f2a17d3e1ecf5c2eafe')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Kazan.dgdat" "${pkgdir}/opt/2gis/kazan.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Kazan.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/kazan.dglf" || return 1
}
