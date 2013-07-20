Boost
=====

http://www.boost.org/users/history/version_1_54_0.html

Configuration:

```bash
./b2 -sICU_PATH=/opt/icu define=U_STATIC_IMPLEMENTATION=1 toolset=gcc variant=release link=static threading=multi runtime-link=static stage release address-model=64 --layout=versioned cxxflags=-fPIC -j4
```

Built with GCC 4.1.2 under Debian/Etch for:

* Linux/amd64 
* Linux/i386
