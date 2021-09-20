FROM devkitpro/devkitppc@sha256:b4c7622442bef192fa13ef34ec90741820cef2fb0c6d6b317a9bd55da06cfa60
RUN dkp-pacman -Syyu --noconfirm && dkp-pacman -Scc --noconfirm
RUN git clone --depth 1 --single-branch -b master https://github.com/devkitPro/wut && cd wut && git reset --hard eb0306184d46a63d929aede352f54109701b7112 && make install && cd .. && rm -rf wut