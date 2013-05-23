# Maintainer : boronology
pkgname=ttf-kacho
pkgver=2011
pkgrel=1
depends=('fontconfig' 'xorg-font-utils')
makedepends=('convmv')
pkgdesc="handwritten-like Japanese fonts set \"花鳥風月\" provided by TAKAYA"
arch=('any')
# License URL : http://www.geocities.jp/s318shunkasyuto/syoukai/syoukai.html
license=('custom')
url="http://www.geocities.jp/s318shunkasyuto/"
source=(http://www.geocities.jp/s318shunkasyuto/down/font/katyou.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoup.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoub.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoubb.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoupb.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoupbb.zip)

install=$pkgname.install

package() {
	  cd $srcdir
	  convmv -f cp-932 -t utf-8 --notest ./*.ttf
	  install -Dm644 花鳥風月.ttf "$pkgdir/usr/share/fonts/TTF/kacho.ttf"
	  install -Dm644 花鳥風月Ｂ.ttf "$pkgdir/usr/share/fonts/TTF/kachob.ttf"
	  install -Dm644 花鳥風月ＢＢ.ttf "$pkgdir/usr/share/fonts/TTF/kachobb.ttf"
	  install -Dm644 花鳥風月Ｐ.ttf "$pkgdir/usr/share/fonts/TTF/kachop.ttf"
	  install -Dm644 花鳥風月ＰＢ.ttf "$pkgdir/usr/share/fonts/TTF/kachopb.ttf"
	  install -Dm644 花鳥風月ＰＢＢ.ttf "$pkgdir/usr/share/fonts/TTF/kachopbb.ttf"}

md5sums=('de7039d132eea3279ccfa5b4e5554eee'
         'db85046cab69b0000f8a56b23cbc352b'
         'f5ecce4f1590e986276fe1a0680c2b1e'
         'ed49251a0878d96173cb23dd76293242'
         '590983afe56f1ae1f171e16118469a5d'
         '32eef2ff1ade6623e1c06db28095186d')
