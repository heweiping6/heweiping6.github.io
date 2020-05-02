### sed

https://ftp.gnu.org/gnu

https://ftp.gnu.org/gnu/sed/sed-4.7.tar.xz

```bash
./configure  --prefix=$HEWEIPING6/sed
make install
```

### coreutils

https://ftp.gnu.org/gnu

https://ftp.gnu.org/gnu/coreutils/coreutils-8.30.tar.xz

```bash
./configure  --prefix=$HEWEIPING6/coreutils
make install
```

### python

https://www.python.org

https://www.python.org/ftp/python/3.7.6/Python-3.7.6.tgz

```bash
./configure  --prefix=$HEWEIPING6/python3.7.6
make install
```


### Pkg-config

https://www.freedesktop.org/wiki/Software/pkg-config/

https://pkg-config.freedesktop.org/releases/pkg-config-0.29.2.tar.gz

```bash
./configure  --prefix=$HEWEIPING6/pkg-config  --with-internal-glib
make -j 4 install
```

### autoconf

https://ftp.gnu.org/gnu/autoconf/autoconf-2.69.tar.gz

```bash
./configure --prefix=$HEWEIPING6/autoconf
make -j 4 install
```

### autmake

https://ftp.gnu.org/gnu/automake/automake-1.16.tar.gz

```bash
./configure --prefix=$HEWEIPING6/automake
make -j 4 install
```

### vim

https://www.vim.org/sources.php

ftp://ftp.vim.org/pub/vim/unix/vim-8.1.tar.bz2

```bash
./configure --prefix=$HEWEIPING6/vim
make -j 4 install
```

### java jre

https://sdlc-esd.oracle.com/ESD6/JSCDL/jdk/8u241-b07/1f5b5a70bf22433b84d0e960903adac8/jre-8u241-macosx-x64.dmg?GroupName=JSC&FilePath=/ESD6/JSCDL/jdk/8u241-b07/1f5b5a70bf22433b84d0e960903adac8/jre-8u241-macosx-x64.dmg&BHost=javadl.sun.com&File=jre-8u241-macosx-x64.dmg&AuthParam=1582371021_8c73276fdf63c3a51f1d1241948b807c&ext=.dmg

https://www.oracle.com/java/technologies/javase-jdk13-downloads.html

jdk

https://download.oracle.com/otn-pub/java/jdk/13.0.2+8/d4173c853231432d94f001e99d882ca7/jdk-13.0.2_osx-x64_bin.dmg?AuthParam=1582381325_393dfdb3708fb4fbde3fd789821b4374

```bash
java --version
java 13.0.2 2020-01-14
Java(TM) SE Runtime Environment (build 13.0.2+8)
```

### cpio

https://ftp.gnu.org/gnu/cpio/cpio-2.13.tar.gz
```bash
./configure --prefix=$HEWEIPING6/cpio
make -j 4 install
```

### eclipse

http://ftp.yz.yamagata-u.ac.jp/pub/eclipse/oomph/epp/2019-12/R/eclipse-inst-mac64.dmg


### gawk

https://ftp.gnu.org/gnu/gawk/gawk-5.0.1.tar.gz

```bash
./configure --prefix=$HEWEIPING6/gawk
make -j 4 install
```

### zlib

http://zlib.net

http://zlib.net/zlib-1.2.11.tar.xz

```bash
./configure --prefix=$HEWEIPING6/zlib
make -j 4 install
```

### nettle

https://www.lysator.liu.se/~nisse/nettle/
https://ftp.gnu.org/gnu/nettle/nettle-3.5.tar.gz

```bash
./configure --prefix=$HEWEIPING6/nettle
make -j 4 install
```

### gmp

https://gmplib.org

https://gmplib.org/download/gmp/gmp-6.2.0.tar.xz

```bash
./configure --prefix=$HEWEIPING6/gmp
make -j 4 install
```

### libtool

https://ftp.gnu.org/gnu/libtool/libtool-2.4.6.tar.gz

```bash
./configure --prefix=$HEWEIPING6/libtool
make -j 4 install
```


### libunistring

https://ftp.gnu.org/gnu/libunistring/libunistring-0.9.10.tar.gz

```bash
./configure --prefix=$HEWEIPING6/libunistring
make -j 4 install
```

### readline

https://ftp.gnu.org/gnu/readline/readline-8.0.tar.gz

```bash
./configure --prefix=$HEWEIPING6/readline
make -j 4 install
```


### libffi

https://sourceware.org/libffi/

ftp://sourceware.org/pub/libffi/libffi-3.3.tar.gz

```bash
./configure --prefix=$HEWEIPING6/libffi
make -j 4 install
```

### bdw-gc

https://www.hboehm.info/gc/

https://www.hboehm.info/gc/gc_source/gc-8.0.4.tar.gz

```bash
./configure --prefix=$HEWEIPING6/gc
make -j 4 install
```

### guile

https://ftp.gnu.org/gnu/guile/guile-3.0.0.tar.gz

```bash
./configure --prefix=$HEWEIPING6/guile --with-libltdl-prefix=$HEWEIPING6/libtool   --with-libgmp-prefix=$HEWEIPING6/gmp --with-libreadline-prefix=$HEWEIPING6/readline  --with-libunistring-prefix=$HEWEIPING6/libunistring

make -j 4 install
```


### bison

https://mirrors.tuna.tsinghua.edu.cn/gnu/bison/bison-3.5.2.tar.gz

```bash
./configure --prefix=$HEWEIPING6/bison
make -j 4 install
```


dos2unix

https://jaist.dl.sourceforge.net/project/dos2unix/dos2unix/7.4.1/dos2unix-7.4.1.tar.gz

```bash
make prefix=$HEWEIPING6/dos2unix install
```

dos2unix



### gnu-c-manual

https://mirrors.tuna.tsinghua.edu.cn/gnu/gnu-c-manual/gnu-c-manual-0.2.5.tar.gz



======================================================

# under verify.....



autogen

https://ftp.gnu.org/gnu/autogen/rel5.18.16/autogen-5.18.16.tar.gz

```bash
./configure --prefix=$HEWEIPING6/autogen
make -j 4 install
```


gnutls

https://www.gnupg.org/ftp/gcrypt/gnutls/v3.6/
https://www.gnupg.org/ftp/gcrypt/gnutls/v3.6/gnutls-3.6.0.tar.xz
```bash
./configure --prefix=$HEWEIPING6/gnutls
make -j 4 install
```


wget

https://ftp.gnu.org/gnu

https://ftp.gnu.org/gnu/wget/wget-1.20.tar.gz

```bash
./configure  --prefix=$HEWEIPING6/wget
make install
```



https://mirrors.ustc.edu.cn/gnu/gcc/gcc-9.2.0/gcc-9.2.0.tar.gz



glibc 

https://mirrors.ustc.edu.cn/gnu/glibc/glibc-2.29.tar.gz
https://mirrors.ustc.edu.cn/gnu/libc/glibc-2.30.tar.gz
https://mirrors.ustc.edu.cn

```bash
./configure --prefix=$HEWEIPING6/glibc
make -j 4 install
```


qemu

https://download.qemu.org/qemu-4.2.0.tar.xz

```bash
./configure --prefix=$HEWEIPING6/qemu
make -j 4 install
```


glib
http://ftp.gnome.org/pub/GNOME/sources/glib/2.63/glib-2.63.0.tar.xz


```bash
./configure --prefix=$HEWEIPING6/glib
make -j 4 install
```

======================================================

upx


https://github.com/upx/upx/releases/download/v3.96/upx-3.96-src.tar.xz



