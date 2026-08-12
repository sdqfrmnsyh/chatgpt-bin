pkgname=chatgpt-bin
pkgver=26.803.81509
pkgrel=1
pkgdesc="ChatGPT by OpenAI"
arch=('x86_64' 'aarch64')
url="https://developers.openai.com/codex/app"
license=('custom')

source_x86_64=(
    "https://persistent.oaistatic.com/codex-app-prod/linux/rpm/latest/chatgpt.x86_64.rpm"
)

source_aarch64=(
    "https://persistent.oaistatic.com/codex-app-prod/linux/rpm/latest/chatgpt.aarch64.rpm"
)

sha256sums_x86_64=('SKIP')
sha256sums_aarch64=('SKIP')

depends=(
    'glib2'
    'gtk3'
    'nss'
    'libnotify'
    'libxcb'
    'mesa'
    'libglvnd'
    'libx11'
    'libxcomposite'
    'libxdamage'
    'libxext'
    'libxfixes'
    'libxrandr'
    'alsa-lib'
    'at-spi2-core'
    'atk'
    'cairo'
    'openssl'
    'libcups'
    'dbus'
    'libdrm'
    'expat'
    'gcc-libs'
    'gdk-pixbuf2'
    'graphite'
    'nspr'
    'pango'
    'systemd-libs'
    'libusb'
    'libxkbcommon'
    'tar'
    'xdg-utils'
)

package() {
    bsdtar -xf "$srcdir"/*.rpm -C "$pkgdir"
}
