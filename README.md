# Uchronia - time series handling for ensembles simulations and forecasts in C++

This site is an attempt to host jointly several generated API documentations.

## Overview

Uchronia is a C++ library designed to handle multidimensional time series and ensemble thereof. [Uchronia](https://en.wikipedia.org/wiki/Uchronia) is a literary neologism for a hypothetical or fictional time-period of our world. This seems a suitable name for a library primarily designed notably to handle retrospective ensemble forecast time series.

See also a [blog post on this case study](https://jmp75.github.io/work-blog/documentation/c++/python/mkdocs/2022/08/22/doxygen-doxybook-mkdocs.html)

## Draft notes

`sudo apt install doxygen`

### Installing doxybook2

```sh
git clone --depth=1 https://github.com/matusnovak/doxybook2.git
ls
cd doxybook2/
```

```sh
git clone https://github.com/microsoft/vcpkg
./vcpkg/bootstrap-vcpkg.sh
```

A bit of adjustment for compiling doxygen2, compared to what the github repo readme says:

```sh
cmake -B ./build -G "Unix Makefiles"     -DCMAKE_BUILD_TYPE=MinSizeRel     -DCMAKE_TOOLCHAIN_FILE=${HOME}/src/vcpkg/scripts/buildsystems/vcpkg.cmake
cmake --build ./build --config MinSizeRel  # could do with a -j4 perhaps
${HOME}/src/doxybook2/build/src/DoxybookCli/doxybook2 --help
```

```sh
DX2=${HOME}/src/doxybook2/build/src/DoxybookCli/doxybook2
```

MkDocs + Material theme - example/mkdocs-material/.doxybook/config.json adapted.

cpp relative url because we aim to host not only cpp. Try, at least.

config-doxybook2.json has ` "baseUrl": "/cpp/",`

Doxyfile:

don't want full machine-specific paths shown, and C API pattern marker

```text
FULL_PATH_NAMES        = NO

INPUT_FILTER           = "sed 's/DATATYPES_API//'"

```

Note: perhaps `STRIP_FROM_PATH` instead?

```sh
doxygen Doxyfile

mkdir -p docs/cpp
$DX2 --input ./doxyoutput/xml --output ./docs/cpp --config config-doxybook2.json
```

```sh
. ~/config/baseconda
conda activate poetry
mkdocs build --clean --site-dir _build/html --config-file mkdocs.yml
mkdocs serve
```

```sh
mkdocs gh-deploy --clean --site-dir _build/html --config-file mkdocs.yml
```

## Python code

Checking that indeed, the `mkdocs.yml` and `docs/` folder are enough to run mkdocs so long as the package is accessible in the virtual environment. Not sure whether having them installed in `develop` mode is required for it to work, but given that docstrings would be present even in a normal installation, probably all right in all cases.

