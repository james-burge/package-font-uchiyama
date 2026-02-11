# Maintainer: Your Name <your.email@example.com>
pkgname=uchimaya-font
pkgver=1.0
pkgrel=1
pkgdesc="A clean, modern Japanese font."
arch=('any')
license=('OFL')
url="https://github.com/james-burge/package-font-uchimaya"
depends=('fontconfig')
source=("file://${HOME}/Projects/package-font-uchiyama/uchiyama.otf")
sha256sums=('SKIP')  # Use SKIP since we are using a local file

package() {
  # Create the target directory for the font
  mkdir -p "$pkgdir/usr/share/fonts/OTF"

  # Copy the font file from the source to the package directory
  cp "${srcdir}/uchiyama.otf" "$pkgdir/usr/share/fonts/OTF/"

  # Rebuild the font cache
  fc-cache -fv
}
