pkgname=gitbook-editor
pkgver=6.2.0
pkgrel=1
pkgdesc="An editor to write and publish books"
arch=('x86_64')
category=Office
url="https://www.gitbook.com/editor"
license=('custom')
source=("http://downloads.editor.gitbook.com/download/linux-64-bit")
depends=("gtk2" "gconf" "nss" "libnotify" "alsa-lib")
md5sums=('396d1ba9908be21e06dbc02e32ee79cb')

package(){
tar -xf data.tar.xz -C $pkgdir
install -Dm664 $pkgdir/opt/gitbook-editor/icon.png $pkgdir/usr/share/pixmaps/gitbook-editor.png
sed -i "s|Categories=Application|Categories=Office|" $pkgdir/usr/share/applications/gitbook-editor.desktop
}
