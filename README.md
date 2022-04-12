# docker-cross-compiler
minimal bare metal cross compiler in docker environment

# How to use
```
docker pull chent11/cross-compiler:cortex_m4-nano_newlib-hf
echo 'docker run --rm chent11/cross-compiler:cortex_m4-nano_newlib-hf "@"' > docker-cmd
chmod +x docker-cmd
./docker-cmd make
```

| Docker Image                                    | CPU       | FPU-Enabled |  Size  |
|-------------------------------------------------|-----------|-------------|--------|
| chent11/cross-compiler:cortex_m4-nano_newlib-hf | cortex-m4 | Yes         | 567 MB |
