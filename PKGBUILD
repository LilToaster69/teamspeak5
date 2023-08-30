maintainer="DarkToaster <info@darkly.biz>"
pkgname=teamspeak5
pkgver=5.0.0beta74
pkgrel=1
pkgdesc="TEST THE FUTURE OF GAMING COMMUNICATION

The all-new TeamSpeak Client is built on the foundations of our rock solid, lag-free voice technology and packed with next-generation communication & productivity tools, while maintaining our renowned security and privacy.

TeamSpeak is the ONLY tool you will need to connect online.
"
arch=('x86_64')
url="https://teamspeak.com/en/downloads/#ts5"
license=('custom')
depends=('libc++' 'libxkbcommon' 'libxslt' 'libxss' 'nss' 'xcb-util-image' 'xcb-util-keysyms' 'xcb-util-renderutil' 'xcb-util-wm' 'libolm' 'libgles' 'libegl')
source=("https://files.teamspeak-services.com/pre_releases/client/5.0.0-beta74/teamspeak-client.tar.gz"
        "https://darksys.pw/aur/teamspeak5/teamspeak5.desktop")
sha256sums=('06d65e5ae8e479965ae6eb2517fd8e7beedca1c774acecfe87830c0338e9e373'
            'cbb865d429ffc0f3ec4a4caa3b95ec09a8665ccf2f7e56b1c4ae127a8d1db2d6')

package() {
    install -dm755 "$pkgdir/opt/teamspeak5"
    cp -r "$srcdir"/* "$pkgdir/opt/teamspeak5/"
    chmod 755 "$pkgdir/opt/teamspeak5/TeamSpeak"

    install -D -m644 "$srcdir/teamspeak5.desktop" \
        "${pkgdir}/usr/share/applications/teamspeak5.desktop"
}

