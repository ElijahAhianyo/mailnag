# Maintainer: Patrick Ulbrich <zulu99 at gmx . net>
# Contributor: rasmus <rasmus . pank at gmail . com>

pkgname=mailnag
pkgver=0.9.9
pkgrel=1
pkgdesc="An extendable mail notification daemon."
arch=('any')
url="https://github.com/pulb/mailnag"
license=('GPL')
depends=('python2' 'python2-gobject' 'python2-httplib2'
        'libgnome-keyring' 'gnome-keyring' 'python2-xdg'
        'python2-dbus' 'libnotify' 'gstreamer0.10-base-plugins')
makedepends=('gettext')
source=('https://github.com/pulb/mailnag/archive/0.9.9-testing.tar.gz')
md5sums=('b8c0986641ac9c911dd3ae62df3187d7')
install='mailnag.install'

build() {
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}-testing"
  python2 setup.py install --root=${pkgdir}
  install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}