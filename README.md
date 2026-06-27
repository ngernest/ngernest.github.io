# ngernest.github.io

This repo contains the source code for `ngernest.github.io`, 
built using [Soupault](https://soupault.app), a static site generator written in OCaml. 

## Building
* Make sure you're using an Opam switch with OCaml 5.0.0 installed!
* Make sure soupault 4.0.0 or later is installed on your system. (Earlier versions of Soupault will not work as they expect a different config file format.)
  * If not, run `opam install soupault`.
* Install Pandoc via `brew install pandoc` 
* Run `soupault` in the top-level directory.
* Serve the `docs/` directory (e.g. with `python3 -m http.server --directory docs`) and visit the page at `http://localhost:8000/`.




 
