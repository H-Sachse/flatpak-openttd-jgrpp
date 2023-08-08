# org.openttd.OpenTTD
Fork of flathub's openttd build repository adding JGRennison's patch pack

prepare:
 - git clone https://github.com/H-Sachse/org.openttd.OpenTTD
 - git checkout jgrpp
 - git submodule init
 - git submodule update

compile
 - flatpak-builder --force-clean build-dir com.github.JGRennison.OpenTTD-jgrpp.yaml

install
 - flatpak-builder --user --install --force-clean build-dir com.github.JGRennison.OpenTTD-jgrpp.yaml

run
 - flatpak run com.github.JGRennison.OpenTTD-jgrpp
