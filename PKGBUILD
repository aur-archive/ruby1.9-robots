# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Babken Vardanyan <483ken@gmail.com>

_gemname=robots
pkgname=ruby1.9-$_gemname
pkgver=0.10.1
pkgrel=1
pkgdesc='Simple robots.txt parser'
arch=(any)
url='http://github.com/fizx/robots'
license=()
depends=(ruby1.9)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('c73cd202dc53972f027a634f4b17e9556ac1255c')

package() {
  local _gemdir="$(ruby-1.9 -e'puts Gem.default_dir')"
  gem-1.9 install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
