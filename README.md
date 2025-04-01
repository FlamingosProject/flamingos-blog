# Flamingos Blog
Philipp Oppermann and Bart Massey 2025

This is the blog for Flamingos, a tutorial Rust OS for small
devices.

## Building

To build this book, install `mdbook` and our patched version
of `mdbook-rss`:

```shell
cargo install mdbook
cargo install --git https://gitlab.com/bartmassey-upstream/mdbook-rss \
  --branch fixes-2025 mdbook-rss
```

Then run `mdbook build`.
