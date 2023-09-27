# PyMOL-Wasm
This is a repository providing a binary and html/javascript code for WebAssembly port of PyMOL.

* This project is based on pymol-open-source. [pymol-open-source](https://github.com/schrodinger/pymol-open-source)
* The source code was slightly modified to make it compatible with emscripten and WebGL.
* The modified source code will be available soon in different repository.

# License

* The pymol part follows original PyMOL's license: [See this](https://github.com/schrodinger/pymol-open-source/blob/master/LICENSE)
* The frontend part (Javascript and html) follows MIT license.

# Demonstration page
* Visit here: [Quite a simple demo page](https://yakomaxa.github.io/PyMOL-Wasm/)

# Current Limitation

* Selection by clicking behave slightly different from original PyMOL. Try moving the pointer after clicking.
* Too large structures cannot be loaded.
* The resizing window after launching PyMOL makes the click-position recogntion wrong.
* The dot representation is very weak to see and very heavy to load.
* Trying to show the cell (unit cell) crashes the session.

# Dependency and requirements for building 

* [pymol-open-source](https://github.com/schrodinger/pymol-open-source) 
* [gl4es](https://github.com/ptitSeb/gl4es)
* [exodide](https://github.com/ymd-h/exodide)
* [pyodide](https://github.com/pyodide/pyodide)

# How this works

* PyMOL source code was built into whl by emscripten with help of exodide.
* The whl is loaded by Pyodide.
* Pyodide executes pymol commands called by Javascript.
* Javascript controls which pymol commands should be executed.

# Feedbacks

* We appreciate your feedbacks to improve this project.
