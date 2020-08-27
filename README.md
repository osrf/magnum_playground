A place to play with the Magnum rendering engine.

https://magnum.graphics/

## Magnum installation

Install the Corrade dependency (part of the Magnum project):

```
mkdir -p ~/workspace && cd ~/workspace
git clone https://github.com/mosra/corrade.git
cd corrade
mkdir build && cd build
cmake -DCMAKE_INSTALL_PREFIX=/usr ..
make -j
sudo make -j install
```

Clone the Magnum repository:

```
mkdir -p ~/workspace && cd ~/workspace
git clone https://github.com/mosra/magnum.git
cd magnum
git checkout v2020.06
```

Compile Magnum:

```
mkdir build && cd build
cmake -DCMAKE_INSTALL_PREFIX=/usr -DWITH_SDL2APPLICATION=ON ..
make -j
sudo make -j install
```

For testing, download the magnum-bootstrap project:

```
mkdir -p ~/workspace && cd ~/workspace
git clone https://github.com/mosra/magnum-bootstrap.git
cd magnum-bootstrap
git checkout base
```

Compile magnum-bootstrap:

```
mkdir build && cd build
cmake ..
make -j
```

And run our first application:

```
./src/MyApplication
```

![A first sample](images/magnum-bootstrap.png)

References:
  * [Building Corrade](https://doc.magnum.graphics/corrade/building-corrade.html#building-corrade-manual)
  * [Building Magnum](https://doc.magnum.graphics/magnum/building.html#building-manual)
  * [Building and running magnum-bootstrap](https://doc.magnum.graphics/magnum/getting-started.html)

