# Maintainer: leafduo <leafduo@gmail.com>
pkgname=linuxqq
pkgver=1.0_Preview2008
pkgrel=1
pkgdesc="QQ for Linux 1.0 Preview"
url="http://www.qq.com/"
license=("")
depends=('gtk2>=2.10')
arch=(i686 x86_64)
makedepends=('tar')
source=(http://dl_dir.qq.com/linuxqq/linuxqq_1.0-Preview2008_i386.deb)
md5sums=('b392c46c20fb9acd507e9dd4f83c2906')
build() {
    cd $startdir/src/
    ar vx linuxqq_1.0-Preview2008_i386.deb
    tar xfz data.tar.gz
    chmod 0755 $startdir/src/usr/bin/QQ $startdir/src/usr/share/apps/Tencent/QQ/*
    cp -a $startdir/src/usr $startdir/pkg
    ln -s /usr/bin/QQ $startdir/pkg/usr/bin/qq
}
