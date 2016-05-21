# python-rust-fst

Python bindings for [burntsushi's][1] [fst crate][2] ([rustdocs][3])
for FST-backed sets and maps.

Currently only a subset of the `Set` functionality is exposed.

For reasons why you might want to consider using it, see BurntSushi's great
article on ["Index[ing] 1,600,000,000 Keys with Automata and Rust"][4].

**tl;dr**:
- Work with larger-than-memory sets
- Perform fuzzy search using Levenshtein automata

## Installation
- You will need:
    * Python 3 with development headers installed
    * Rust nightly (install via [rustup][5])
- Clone the repository. Installation with `pip install git+...` does not work
  currently
- Add `rustup override add nightly` to add an override for rustup to use the
  nightly channel for the repository
- Run `python setup.py bdist_wheel` to generate a wheel
- Install the wheel with `pip install dist/rust_fst-0.1-py3-none-any.whl`

[1]: http://blog.burntsushi.net/transducers/
[2]: https://github.com/BurntSushi/fst
[3]: http://burntsushi.net/rustdoc/fst/
[4]: http://blog.burntsushi.net/transducers/
[5]: https://www.rustup.rs/
