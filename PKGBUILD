# Contributor: DigitalPathogen <aur@InfoSecResearchLabs.co.uk>

pkgname=enum4linux
pkgver=0.8.4
pkgrel=1
pkgdesc="a tool for enumerating information from Windows and Samba systems."
arch=('i686' 'x86_64')
url="http://labs.portcullis.co.uk/application/enum4linux/"
license=('GPL')
depends=('perl' 'polenum' 'smbclient')
source=(http://labs.portcullis.co.uk/download/$pkgname-$pkgver.tar.gz)
md5sums=('40e99278d5025b69a947aaa182761833')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  install -D -m 0755 -o root -g root enum4linux.pl ${pkgdir}/usr/bin/enum4linux.pl
  install -D -m 0644 -o root -g root share-list.txt ${pkgdir}/usr/share/enum4linux/share-list.txt
}

# vim:set ts=2 sw=2 et:
