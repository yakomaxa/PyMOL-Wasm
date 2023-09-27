# PyMOL-Wasm
This is a repository providing binary and html/javascript code for WebAssembly port of PyMOL.

* This project is based on pymol-open-source. [pymol-open-source](https://github.com/schrodinger/pymol-open-source)
* The source code is slightly modified to make it compatible with emscripten and WebGL.
* The modified source code will be available soon in different repository.

# License

* The pymol part follows PyMOL's license [See this](https://github.com/schrodinger/pymol-open-source/blob/master/LICENSE)
* The frontend part (Javascript and html) follows MIT license.

# Demonstration page
* Vist here: [Quite a simple demo page](https://yakomaxa.github.io/PyMOL-Wasm/)

# Current Limitation

* Too large structures cannot be loaded.
* The resizing window after launching PyMOL makes the click-position recogntion.
* The dot representation is very weak to see.
* Trying to show the cell (unit cell) crashes the session
