FROM devkitpro/devkitppc:20220216

RUN git clone --depth 1 --single-branch -b master https://github.com/devkitPro/wut && cd wut && git reset --hard cd6b4fb45d054d53af92bc0b3685e8bd9f01445d && make install && cd .. && rm -rf wut