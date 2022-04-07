# docker-cross-compiler
minimal bare metal cross compiler in docker environment

# How to use
```
docker pull chent11/cross-compiler:cortex-m4-hf
echo 'docker run --rm chent11/cross-compiler:cortex-m4-hf "@"' > docker-cmd
chmod +x docker-cmd
./docker-cmd make
```

| Docker Image                        | CPU       | FPU-Enabled | Size  |
|-------------------------------------|-----------|-------------|-------|
| chent11/cross-compiler:cortex-m4-hf | cortex-m4 | Yes         | 596MB |
