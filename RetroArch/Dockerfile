FROM retrostick-base

RUN git clone -b v1.19.1 --single-branch --depth 1 https://github.com/libretro/RetroArch.git

COPY patch/Makefile.gslv5 ./RetroArch/

COPY patch/*.patch compile.sh ./

ENTRYPOINT ["bash", "/build/compile.sh"]
