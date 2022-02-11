FROM devkitpro/devkitppc@sha256:b4c7622442bef192fa13ef34ec90741820cef2fb0c6d6b317a9bd55da06cfa60
RUN ln -sf /proc/mounts /etc/mtab
RUN dkp-pacman -Syyu --noconfirm && dkp-pacman -Scc --noconfirm
RUN git clone --depth 1 --single-branch -b master https://github.com/devkitPro/wut && cd wut && git reset --hard 888bab16b5e74a09d0c4d219607f65cc44e7b4ec && make install && cd .. && rm -rf wut