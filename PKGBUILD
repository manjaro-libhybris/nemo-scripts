# Maintainer: Bardia Moshiri <fakeshell@bardia.tech>

pkgname=nemo-scripts
pkgver=0.1
pkgrel=1
pkgdesc="scripts to get nemomobile running"
arch=('any')
url="https://github.com/manjaro-libhybris/nemo-scripts"
license=('custom')
depends=('systemd' 'sudo')
source=('nemo-scripts::git+https://github.com/manjaro-libhybris/nemo-scripts')
sha256sums=('SKIP')

package() {
    cd nemo-scripts
    install -Dm644 "etc/glacier/blacklistapp" "${pkgdir}/etc/glacier/blacklistapp"
    install -Dm644 "etc/hw-release" "${pkgdir}/etc/hw-release"
    install -Dm644 "etc/pulse/xpolicy.conf" "${pkgdir}/etc/pulse/xpolicy.conf"
    install -Dm755 "usr/bin/nemomobile" "${pkgdir}/usr/bin/nemomobile"
    install -Dm644 "var/lib/environment/compositor/manjaro.conf" "${pkgdir}/var/lib/environment/compositor/manjaro.conf"
    install -Dm644 "var/lib/environment/nemo/70-manjaro.conf" "${pkgdir}/var/lib/environment/nemo/70-manjaro.conf"
    install -Dm644 "var/lib/environment/nemo/manjaro.conf" "${pkgdir}/var/lib/environment/nemo/manjaro.conf"
    install -Dm644 "usr/lib/systemd/system/nemomobile.service" "${pkgdir}/usr/lib/systemd/system/nemomobile.service"
}
