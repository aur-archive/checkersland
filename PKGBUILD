# Maintainer: archtux <antonio dot arias99999 at gmail dot com>

pkgname=checkersland
pkgver=4.4
pkgrel=1
pkgdesc="Сheckers program with 31 variants for playing with computer or people via the Internet."
arch=('any')
url="http://www.checkersland.com/download/pc.jsp"
license=('GPL3')
depends=('java-runtime')
source=(http://www.checkersland.com/download/$pkgname.jar
        $pkgname.desktop
        $pkgname.jpeg
        $pkgname.sh)
md5sums=('bf51b1944ba65df6ee2e34a5938a98f2'
         '38278b910c48edfa05a0477659e91611'
         '04eacd617e76d6a34931a23b81d0b8f7'
         '1a478f28c458c13e87cd06be54394cea')

package() {
  cd $srcdir
  # Executable
  install -Dm755 $pkgname.jar $pkgdir/usr/share/$pkgname/$pkgname.jar

  # Start file
  install -Dm755 $pkgname.sh $pkgdir/usr/bin/$pkgname
  
  # Desktop icon
  install -Dm644 $pkgname.jpeg $pkgdir/usr/share/pixmaps/$pkgname.jpeg
  install -Dm644 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
