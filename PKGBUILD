# Maintainer: Anonymous
pkgname=wps-office-bwrap
pkgver=1.0
pkgrel=4 # <-- 递增此处的构建号以触发系统更新
pkgdesc="use bubblewrap sandbox to stop wpscloudsvr (Fixed IPC & Multi-directory support)"
arch=('any')
url="https://blog.ruo-chen.wang/2021/08/bwrap-wps.html"
license=('custom')
depends=('wps-office' 'bubblewrap')

# 确保你的工作目录下有这俩文件
source=('wps-bwrap'
  'wps-office-bwrap.desktop')

sha256sums=('SKIP'
  'SKIP')

package() {
  install -d "${pkgdir}/usr/bin"
  install -d "${pkgdir}/usr/share/applications"

  install -m755 "${srcdir}/wps-bwrap" "${pkgdir}/usr/bin/wps-bwrap"
  install -m644 "${srcdir}/wps-office-bwrap.desktop" "${pkgdir}/usr/share/applications/wps-office-bwrap.desktop"
}
