pkgname=ttf-opentui-mono
pkgver=34.4.0 # Iosevka version embedded in the fonts
pkgrel=1
pkgdesc='OpenTUI Mono, a custom Iosevka build (static TTF, unhinted)'
arch=(any)
url='https://github.com/anomalyco/opentui'
license=(OFL-1.1)
provides=(ttf-font)

# shortcut: installs the committed ttf/ files from this checkout, no source download; for the AUR switch to a git source
package() {
  install -Dm644 -t "$pkgdir/usr/share/fonts/TTF" "$startdir"/ttf/*.ttf
  install -Dm644 "$startdir/LICENSE.md" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
