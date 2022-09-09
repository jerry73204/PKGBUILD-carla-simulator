# Maintainer: Jerry Lin <jerry73204@gmail.com>
pkgname=carla-simulator-bin
pkgver=0.9.13
pkgrel=1
epoch=
pkgdesc='CARLA is an open-source simulator for autonomous driving research.'
arch=('x86_64')
url='https://carla.org/'
license=('MIT')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=('carla-simulator')
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(
  "https://carla-releases.s3.eu-west-3.amazonaws.com/Linux/CARLA_${pkgver}.tar.gz"
  "https://carla-releases.s3.eu-west-3.amazonaws.com/Linux/CARLA_${pkgver}_RSS.tar.gz"
  "https://carla-releases.s3.eu-west-3.amazonaws.com/Linux/AdditionalMaps_${pkgver}.tar.gz"
)
b2sums=(
  '8998a2de74f84f76569d7cd8e925b877c58fa25eb0d4dda2d0a762f8bba30985bcb60eb4ab66a8949091d60db92385e406d6b88b1f07a1a26b3d37dbdad5aa4f'
  'a6df9fc13d5282bb193aefdfacde4f0c0374c38d9147ec40a1eecf8d7ce87b88773308a02dea26ed2bc0e4210356fdd103e75a3580836f95bdf163b3f4cff4dc'
  '1a0119a8cb5fbcb8c28326c9c1d65785535fd34af7f70e47c67705fec470c1cd857028e5fb34f5d2e437e6dd9540d9810f139133b994b1a2021c6c22bfc19da7'
)
noextract=(
  "CARLA_${pkgver}.tar.gz"
  "CARLA_${pkgver}_RSS.tar.gz"
  "AdditionalMaps_${pkgver}.tar.gz"
)
validpgpkeys=()

package() {
  carla_dir="$pkgdir/opt/carla-simulator"
  mkdir -p "$carla_dir"
  bsdtar -x -C "$carla_dir" -f "${srcdir}/CARLA_${pkgver}.tar.gz"
  bsdtar -x -C "$carla_dir" -f "${srcdir}/CARLA_${pkgver}_RSS.tar.gz"
  bsdtar -x -C "$carla_dir" -f "${srcdir}/AdditionalMaps_${pkgver}.tar.gz"
}
