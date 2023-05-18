# Maintainer: Bardia Moshiri <fakeshell@bardia.tech>

pkgname=nemo-scripts
pkgver=1
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
    install -Dm644 "etc/pulse/arm_droid_card_custom.pa" "${pkgdir}/etc/pulse/arm_droid_card_custom.pa"
    install -Dm644 "etc/systemd/system/usb-tethering.service.d/10-connman.conf" "${pkgdir}/etc/systemd/system/usb-tethering.service.d/10-connman.conf"
    install -Dm644 "etc/ofono/dbusaccess.conf" "${pkgdir}/etc/ofono/dbusaccess.conf"
    install -Dm644 "usr/lib/systemd/system/nemomobile.service" "${pkgdir}/usr/lib/systemd/system/nemomobile.service"
    install -Dm755 "usr/bin/nemomobile" "${pkgdir}/usr/bin/nemomobile"
    install -Dm644 "var/lib/environment/compositor/manjaro.conf" "${pkgdir}/var/lib/environment/compositor/manjaro.conf"
    install -Dm644 "var/lib/environment/nemo/70-manjaro.conf" "${pkgdir}/var/lib/environment/nemo/70-manjaro.conf"
    install -Dm644 "var/lib/environment/nemo/manjaro.conf" "${pkgdir}/var/lib/environment/nemo/manjaro.conf"
}
