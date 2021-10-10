pkgname=archlinux-keyring-archzfs
pkgver=20180709
pkgrel=1
pkgdesc='ArchZFS PGP keyring'
arch=(any)
url=https://zfsonlinux.org/
license=(CDDL)

depends=(archlinux-keyring)
install=archzfs.install

source=(archzfs{.gpg,-revoked,-trusted})

sha512sums=('01f6d4dcf4ee0db273378b27dc3217bf1b29c7f3a05b86cafd63076093972620ba5557f37c19db8276f0ef9a9963e285e43d99d7d407fb455e0cb3df71dbe844'
            'cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e'
            'cf66ad4a231c8e47272fa8b218a7d67e0720d751ac4dbb760ec08f2f3f212cabf7f56a9e392abd2a5214757719b6b274c6bd6f23d0471cddbfe8f7ad1f0603ad')
b2sums=('d061fce745b4174e5ac1a7c7d57addf004041ab2c7476c9564c534e1a79cee10bc08ab0f256887fed69567bc62fa390915bb25ce55f1321ca72f0ba53336ff03'
        '786a02f742015903c6c6fd852552d272912f4740e15847618a86e217f71f5419d25e1031afee585313896444934eb04b903a685b1448b755d56f701afe9be2ce'
        '0010c657066faa0378afd3d2fc1fd3ef042c68bf393f7eb1c74db2172aff8f44565956e3fe89b5433b41ce09227f24d53bbaa4319ab6843901aa9640dc4acf6f')

package() {
    install -Dm644 -t ${pkgdir}/usr/share/pacman/keyrings "${source[@]}"
}
