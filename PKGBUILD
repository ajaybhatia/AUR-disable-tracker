# Maintainer: Ajay Bhatia

pkgname=disable-tracker
pkgver=0.1
pkgrel=3
pkgdesc="Script for disabling tracker in gnome session"
arch=(any)
url="https://github.com/Chrysostomus/$pkgname"
license=(MIT)
makedepends=('git')
source=("git://github.com/Chrysostomus/$pkgname")
md5sums=('SKIP')

package () {
	cd "$srcdir"
	install -dm755 $pkgdir/etc/skel/.config/
	cp -r $srcdir/$pkgname/autostart $pkgdir/etc/skel/.config/
    install -Dm755 "$srcdir/$pkgname/disable-tracker.sh" "$pkgdir/usr/bin/disable-tracker.sh"
}
