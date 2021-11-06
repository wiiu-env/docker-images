FROM devkitpro/devkitppc@sha256:b4c7622442bef192fa13ef34ec90741820cef2fb0c6d6b317a9bd55da06cfa60
RUN dkp-pacman -Syyu --noconfirm && dkp-pacman -Scc --noconfirm
RUN git clone --depth 1 --single-branch -b master https://github.com/devkitPro/wut && cd wut && git reset --hard ce2cd4e843391a1658b77ef6f6f4f9f0ca3b386e && make install && cd .. && rm -rf wut