# hello-wasm

Working through Rust + Wasm tutorials with minimal web knowledge aka mostly copy-paste.

## Running

### Install prerequisites

* Rust: <https://rustup.rs>
* wasm-pack: <https://github.com/rustwasm/wasm-pack>

### Build

Use wasm-pack to compile Rust to WASM and generate JS files to interface with the WASM output in a
browser.

```sh
wasm-pack build --release --target web
```

TODO: figure out the equivalent flow using Webpack.

### Start a server

#### Option 1: Using Python's `http.server`

```sh
python3 -m http.server -d app/static 3000
```

#### Option 2: Using the Google Cloud SDK's development server

```sh
dev_appserver.py app/app.yaml --port 3000
```
  
See <https://cloud.google.com/appengine/docs/standard/python/tools/using-local-server> for more.

### View in browser

Open <http://localhost:3000> in your favorite browser

## Resources

* Rust and WebAssembly Documentation: <https://rustwasm.github.io/docs.html>
  * The Rust Wasm Book: <https://rustwasm.github.io/docs/book/introduction.html>
  * The `wasm-bindgen` Guide: <https://rustwasm.github.io/wasm-bindgen/introduction.html>
  * The `wasm-pack` Guide: <https://rustwasm.github.io/docs/wasm-pack>

## Disclaimer

This is not an officially supported Google product (duh)

