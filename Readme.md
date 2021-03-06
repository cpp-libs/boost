Boost
=====

### Usage

```bash
git clone -b 1.55-include --single-branch https://github.com/cpp-libs/boost.git ~/boost/include
git clone -b 1.55-darwin --single-branch https://github.com/cpp-libs/boost.git ~/boost/lib
```

### Version [1.54](https://github.com/cpp-libs/boost/tree/1.54-include "v1.54 headers") ([linux/i386](https://github.com/cpp-libs/boost/tree/1.54-linux_x86 "linux/i386"), [linux/amd64](https://github.com/cpp-libs/boost/tree/1.54-linux_amd64 "linux/amd64"))

http://www.boost.org/users/history/version_1_54_0.html

Configuration:

```bash
./b2 -sICU_PATH=/opt/icu define=U_STATIC_IMPLEMENTATION=1 toolset=gcc variant=release link=static threading=multi runtime-link=static stage release address-model=64 --layout=versioned cxxflags=-fPIC -j4
```

Built with GCC 4.1.2 on Debian/Etch.

### Version [1.55](https://github.com/cpp-libs/boost/tree/1.55-include "v1.55 headers") ([darwin/universal](https://github.com/cpp-libs/boost/tree/1.55-darwin "darwin/universal"))

http://www.boost.org/users/history/version_1_55_0.html

Configuration:

```bash
./b2 -sICU_PATH=/usr/local/icu/52.1 define=U_STATIC_IMPLEMENTATION=1 toolset=darwin variant=release link=static threading=multi runtime-link=static stage release address-model=32_64 --layout=versioned cxxflags="-fPIC -mmacosx-version-min=10.6" -j4
```

Built with XCode 5.0.2 on OS X Mavericks.

(**warning**: does not include libraries for Boost.Context - [ticket #8266](https://svn.boost.org/trac/boost/ticket/8266 "ticket #8266"))

---
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/cpp-libs/boost/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
