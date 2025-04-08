# Flamingos Blog
Philipp Oppermann and Bart Massey 2025

This is the mdbook "source" of the blog for Flamingos, a
tutorial Rust OS for small devices. The blog is at
<https://github.com/flamingosproject.github.io/flamingos-blog>.

## Building

To build this book, install `mdbook` and our patched version
of `mdbook-rss`:

```shell
cargo install mdbook
cargo install --git https://gitlab.com/bartmassey-upstream/mdbook-rss \
  --branch fixes-2025 mdbook-rss
```

Then run `mdbook build`.
