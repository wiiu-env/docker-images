FROM devkitpro/devkitppc:20200730
RUN dkp-pacman -Syu --noconfirm && dkp-pacman -Scc --noconfirm
RUN git clone https://github.com/devkitPro/wut && cd wut && git reset --hard 583b7d412d7e97ef04400071e5836f33682d31d9 && make install && cd .. && rm -rf wut