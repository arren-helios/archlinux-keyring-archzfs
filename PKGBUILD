pkgname=archlinux-keyring-archzfs
pkgver=20241015
pkgrel=2
pkgdesc='ArchZFS PGP keyring'
arch=(any)
url=https://zfsonlinux.org/
license=(CDDL)

depends=(archlinux-keyring)
install=archzfs.install

source=(archzfs{.gpg,-revoked,-trusted})

sha512sums=('6dba18abd66ca0d595adf193cdf0da072513ecc8875b1b27c45bb4d4a2135af80fd7e53ea8e314240a6b30bcff0baa121e36bf83f294cb1e435aba8d16574457'
            'cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e'
            '18446c742eb8aa9904d4ac89324e5c52ac8a5facd4cacf8e098437b14f62900e1ceb02bdc913d1c5acfcf4e814faf109f5f0d94b9dd0b9ee7ec8777f734a705a')
b2sums=('5c5e3e487aedfaba94c679fb47fd6c6c2611739cf434566ac5f7d7ac11e4ad173acfdc50b514c8451374106b7d9ad6ce60d4a1ddd64e1e055e1bce7f21e75ed4'
        '786a02f742015903c6c6fd852552d272912f4740e15847618a86e217f71f5419d25e1031afee585313896444934eb04b903a685b1448b755d56f701afe9be2ce'
        'a23f5c732531c6d620464792eb01f10de4345301312361d7e9f30b1cb8d45f56d1800a9cabbf3dd3cc8a2f6e6a8500061d6aef09ca8c789264153f1249595533')

package() {
    install -Dm644 -t ${pkgdir}/usr/share/pacman/keyrings "${source[@]}"
}
