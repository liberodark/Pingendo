# Maintainer: liberodark

pkgname=pingendo
pkgver=4.0
pkgrel=1
pkgdesc="The ultimate Bootstrap 4 builder"
arch=('x86_64')
url="https://pingendo.com/"
license=('Custom')
depends=('xdg-utils')
source_x86_64=("https://firebasestorage.googleapis.com/v0/b/pingendoauth.appspot.com/o/Pingendo%20${pkgver}-linux64.zip?alt=media")
source=($pkgname.desktop
        $pkgname.png)
sha512sums=('b5ec949c903d2744e886a80c6a0fb33b6b17926c2c9704129819db332a5bfce322c14035413f4c80ec90fbe9855686e6c63d0d7591a3466c5d3755a926e83b88'
         '93cf8eb2d6965f8047a287b4ac81d16fb755a1d85e333364ab5c7725e08bfd6084ab714a5b8b55212e5f29316df149e21c6123b2ffcbc2fff668f01481c877d5')
sha512sums_x86_64=('ec0cdcb5b8af3ffa18241b77c104c72a30cb7ce974a2ba33e7d2da3a46885c15f5553b24dbd0ea9e75e4a70ee8f24b603fd7ab95b71bb683eac35112c47d7d1d')
        
package() {
  cd $srcdir
  mkdir -p "${pkgdir}/opt/pingendo"
  cp -r Pingendo\ 4.0-linux-x64/. "${pkgdir}/opt/pingendo"
  install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}
