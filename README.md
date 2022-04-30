# Junga SoC

Refer to [README](docs/source/quickstart.rst) for a quick start of how to use caravel_user_project

Refer to [README](docs/source/index.rst) for this sample project documentation. 

## Quick Start

 - build
```sh
cd shuttle6/
export PDK_ROOT=$PWD/pdks
export OPENLANE_ROOT=$PWD/openlane

cd caravel_mpw6/
make uncompress
make setup
make user_proj_example
make user_project_wrapper
make compress
```

 - verify
```sh
cd shuttle6/
export PDK_ROOT=$PWD/pdks
export PDK=sky130A
export GCC_PATH=/opt/xpack-riscv-none-embed-gcc/bin
export GCC_PREFIX=riscv-none-embed

cd caravel_mpw6/
make verify
```
