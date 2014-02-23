# Maintainer: Colin Keenan <colinnkeenan at gmail dot com>

pkgname=gmv
pkgver=1.0
pkgrel=1
pkgdesc="GUI for 'mv': Adds 'Move or Rename' to 'open-with' context menu for most files."
arch=('any')
url="https://github.com/colinkeenan/gmv"
license=('GPL')
depends=('yad')       # had to use yad instead of zenity to have default values in forms
install=${pkgname}.install

source=('gmv' 'gmv.desktop')
md5sums=('7e639e2ae25f0953299fd993fff8e13b'
         '5cb898b8e25e883a8a7cb55f84720d5f')

package() {
  install -d -m755 "$pkgdir/usr/bin"
  install -d -m755 "$pkgdir/usr/share/applications"
  install -m755 gmv.desktop "$pkgdir/usr/share/applications"
  install -m755 gmv "$pkgdir/usr/bin/gmv"
}
