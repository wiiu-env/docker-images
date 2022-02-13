FROM wiiu-env/toolchain-base:20220211

RUN ln -sf /proc/mounts /etc/mtab

RUN dkp-pacman -Syyu --noconfirm wiiu-dev && \
    dkp-pacman -S --needed --noconfirm ppc-portlibs wiiu-portlibs && \
    dkp-pacman -S --needed --noconfirm devkitARM && \
    yes | dkp-pacman -Scc

ENV DEVKITPPC=${DEVKITPRO}/devkitPPC
ENV DEVKITARM=/opt/devkitpro/devkitARM

RUN git clone --depth 1 --single-branch -b master https://github.com/devkitPro/wut && cd wut && git reset --hard fefde021b90532b972516fa252beca045f77fe3f && make install && cd .. && rm -rf wut