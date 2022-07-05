# docker-cross-compiler
minimal bare metal cross compiler in docker environment

# How to use
Choose a tag below and pull from repo `chent11/cross-compiler`

Example:
```sh
DOCKER_TAG=cortex_m4-nano_newlib-hf
docker pull chent11/cross-compiler:$DOCKER_TAG
echo 'docker run --rm chent11/cross-compiler:$DOCKER_TAG "@"' > docker-cmd
chmod +x docker-cmd
./docker-cmd make
```

| Image Tags | CPU | FPU | MMU | Uncompressed Image Size |
|:-|:-:|:-:|:-:|:-:|
| ![size](https://shields.io/docker/image-size/chent11/cross-compiler/cortex_m0-nano_newlib)<br/>cortex_m0-nano_newlib | cortex-m0 | ❌ | ❌ | 633M |
| ![size](https://shields.io/docker/image-size/chent11/cross-compiler/cortex_m3-nano_newlib)<br/>cortex_m3-nano_newlib | cortex-m3 | ❌ | ❌ | 0M |
| ![size](https://shields.io/docker/image-size/chent11/cross-compiler/cortex_m4-nano_newlib-hf)<br/>cortex_m4-nano_newlib-hf | cortex-m4 | ✅ | ✅ | 632M |
| ![size](https://shields.io/docker/image-size/chent11/cross-compiler/arm32-nano_newlib-multilibs)<br/>arm32-nano_newlib-multilibs | arm32-multilibs | / | / | 0M |
