# Maintainer: pisuka <tekmon@gmail.com>
_herokuname=heroku-client
pkgname=heroku-toolbelt
pkgver=2.40.0
pkgrel=1
pkgdesc='Everything you need to get started using Heroku'
arch=('i686' 'x86_64')
url='https://toolbelt.heroku.com'
license=('MIT' 'APACHE' 'RUBY' 'PerlArtistic' 'GPL' 'custom')
depends=('ruby>=1.9')
makedepends=('ruby-bundler')
optdepends=('git')
conflicts=('ruby-heroku' 'ruby-foreman' 'heroku-client')
source=(http://assets.heroku.com.s3.amazonaws.com/heroku-client/${_herokuname}.tgz)
md5sums=(SKIP)

package() {
  mkdir -p "$pkgdir/usr/local"
  mv "$srcdir/$_herokuname/" "$pkgdir/usr/local/heroku/"

  mkdir -p "$pkgdir/usr/local/bin"
  ln -s "$pkgdir/usr/local/heroku/bin/heroku" "$pkgdir/usr/local/bin/heroku"
}

# vim:set ts=2 sw=2 et:
