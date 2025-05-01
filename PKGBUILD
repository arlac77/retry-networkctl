pkgname=retry-networkctl
pkgver=1.0.4
pkgrel=0
pkgdesc='reconfigure networkctl until state is online'
arch=(any)
url='https://github.com/arlac77/retry-networkctl.git'
license=(MIT)
public=true

package() {
    depends=(systemd bash)
    install -Dm755 $srcdir/../retry-networkctl "$pkgdir/usr/bin/retry-networkctl"
    install -Dm644 $srcdir/../retry-networkctl.service "$pkgdir/usr/lib/systemd/system/retry-networkctl.service"
}
