FROM devkitpro/devkitppc@sha256:b4c7622442bef192fa13ef34ec90741820cef2fb0c6d6b317a9bd55da06cfa60
RUN dkp-pacman -Syyu --noconfirm && dkp-pacman -Scc --noconfirm
RUN git clone --depth 1 --single-branch -b master https://github.com/wiiu-env/wut && cd wut && git reset --hard f4cd99f1b183c3b471eb29da9b19a78dc842ac91 && make install && cd .. && rm -rf wut