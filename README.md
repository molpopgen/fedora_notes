# Notes on Fedora setup

## Open CL

### Rusticl

Written 23 Jan 2024.

Following [here](https://nullr0ute.com/2023/12/getting-started-with-opencl-using-mesa-rusticl/),

```
sudo dnf install -y mesa-libOpenCL mesa-dri-drivers spirv-llvm-translator spirv-tools-libs clinfo clpeak
```

Then,

```
RUSTICL_ENABLE=radeonsi darktable
```

Currently, we get the black screen problem.
See [here](https://gitlab.freedesktop.org/mesa/mesa/-/issues/7746).

### rocm

Until `rusticl` is sorted, use `rocm-opencl`
