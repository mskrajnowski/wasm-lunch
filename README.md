My playground for preparing a short talk at [10Clouds](http://10clouds.com) about [WebAssembly].
- [WebAssembly](#webassembly)
- [Getting Started](#getting-started)
    - [Emscripten](#emscripten)
    - [WebAssembly Toolkit](#webassembly-toolkit)
    - [C/C++](#cc)
    - [Rust](#rust)
- [Links](#links)
- [Videos](#videos)

# WebAssembly

# Getting Started

## [Emscripten][Emscripten installation]

```sh
wget -q -O - https://s3.amazonaws.com/mozilla-games/emscripten/releases/emsdk-portable.tar.gz | tar xvz 
cd emsdk-portable
./emsdk update
./emsdk install latest
./emsdk activate latest
source emsdk_env.sh
```

## [WebAssembly Toolkit]

```sh
sudo apt-get install cmake build-essential
git clone --recursive https://github.com/WebAssembly/wabt
cd wabt
make gcc-release
```

## [Rust][Rust WebAssembly Installation]

```sh
curl https://sh.rustup.rs -sSf | sh
source $HOME/.cargo/env
rustup install nightly
rustup default nightly
rustup target add wasm32-unknown-emscripten
```

# Links

1. [WebAssembly]
1. [MDN WebAssembly]
1. [Awesome WebAssembly]
1. [WebAssembly Explorer]
1. [WebAssembly Toolkit]
1. [A Cartoon Intro to WebAssembly]
1. [Emscripten]
1. [The Rusty Web]
1. [The Path to Rust on the Web]
1. [TurboScript]
1. [Assembleash]

# Videos

1. [Jay Phelps - WebAssembly Demystified]
1. [WebAssembly Fundamentals]


[WebAssembly]: http://webassembly.org/
[MDN WebAssembly]: https://developer.mozilla.org/en-US/docs/WebAssembly
[Awesome WebAssembly]: https://github.com/mbasso/awesome-wasm
[WebAssembly Explorer]: https://mbebenita.github.io/WasmExplorer/
[WebAssembly Toolkit]: https://github.com/WebAssembly/wabt
[A Cartoon Intro to WebAssembly]: https://hacks.mozilla.org/2017/02/a-cartoon-intro-to-webassembly/
[Emscripten]: http://kripken.github.io/emscripten-site/
[Emscripten Installation]: http://kripken.github.io/emscripten-site/docs/getting_started/downloads.html
[The Path to Rust on the Web]: https://hoverbear.org/2017/04/06/the-path-to-rust-on-the-web/
[The Rusty Web]: https://davidmcneil.gitbooks.io/the-rusty-web/content/
[Rust WebAssembly Installation]: https://davidmcneil.gitbooks.io/the-rusty-web/content/setup-and-hello-world.html
[TurboScript]: https://github.com/01alchemist/TurboScript
[Assembleash]: https://maxgraey.github.io/Assembleash/#TurboScript
[Jay Phelps - WebAssembly Demystified]: https://www.youtube.com/watch?v=cRwUD5SxF4o
[WebAssembly Fundamentals]: https://www.youtube.com/watch?v=jXMtQ2fTl4c
