# Maintainer : boronology
pkgname=ttf-kacho
pkgver=20150615
pkgrel=1
depends=('fontconfig' 'xorg-font-utils')
makedepends=('convmv')
pkgdesc="handwritten-like Japanese fonts set 花鳥風月 provided by TAKAYA"
arch=('any')
license=('custom')
url="http://www.geocities.jp/s318shunkasyuto/"
source=(http://www.geocities.jp/s318shunkasyuto/down/font/katyou.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoup.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoub.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoubb.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoupb.zip
	http://www.geocities.jp/s318shunkasyuto/down/font/katyoupbb.zip
	)

install=$pkgname.install

package() {
	  cd $srcdir
	  convmv -f cp-932 -t utf-8 --notest ./*.ttf
	  install -Dm644 花鳥風月.ttf "$pkgdir/usr/share/fonts/TTF/kacho.ttf"
	  install -Dm644 花鳥風月B.ttf "$pkgdir/usr/share/fonts/TTF/kachob.ttf"
	  install -Dm644 花鳥風月ＢＢ.ttf "$pkgdir/usr/share/fonts/TTF/kachobb.ttf"
	  install -Dm644 花鳥風月Ｐ.ttf "$pkgdir/usr/share/fonts/TTF/kachop.ttf"
	  install -Dm644 花鳥風月PB.ttf "$pkgdir/usr/share/fonts/TTF/kachopb.ttf"
	  install -Dm644 花鳥風月ＰＢＢ.ttf "$pkgdir/usr/share/fonts/TTF/kachopbb.ttf"
	  }

md5sums=('6015d38e5123531b172953ad04c5fb04'
         '0a369b4a0a37a4c6579fa5e91b888b68'
         'f7b4a40e2ca9b3f5b9de897bc1520b8c'
         'cdc1263447b8634a9fbed1ffaa5f3495'
         '5d63a54977416f20c07bf358df8feb32'
         '5ab494c71548ce5ba46e5c86730b5940')
