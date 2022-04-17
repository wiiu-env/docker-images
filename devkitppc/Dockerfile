FROM devkitpro/devkitppc:20220216

RUN git clone --depth 1 --single-branch -b master https://github.com/devkitPro/wut && cd wut && git reset --hard 616ebe1a065d91ac3b394d62de5042b9f8535b0b && make install && cd .. && rm -rf wut