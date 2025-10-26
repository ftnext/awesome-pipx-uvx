# awesome-pipx-uvx
Awesome example of `pipx run` or `uvx`

## Introduction

### uvx

* uv https://docs.astral.sh/uv/
    * >An extremely fast Python package and project manager, written in Rust.
* Installation https://docs.astral.sh/uv/getting-started/installation/
* `uvx` (equivalent `uv tool run`)
    * https://docs.astral.sh/uv/guides/tools/

### pipx (`pipx run`)

* [Installing stand alone command line tools (Python Packaging User Guide)](https://packaging.python.org/en/latest/guides/installing-stand-alone-command-line-tools/)
* Installation https://pipx.pypa.io/stable/installation/
* Pre-installed on GitHub Action's environment (as of January 2025)

## Use cases (ToC)

* [Packaging](#Packaging)
* [Misc](#Misc)

## Packaging

Japanese: https://nikkie-ftnext.hatenablog.com/entry/pipx-run-make-easier-speech-recognition-release-from-codespaces

### Build

```shell
$ uvx build
$ pipx run build
```

### Publish

```shell
$ uvx twine upload dist/*
$ pipx run twine upload dist/*
```

## Misc

### QR code

```shell
$ uvx --from 'qrcode[pil]' qr "Some text" > qr.png
$ pipx run --spec 'qrcode[pil]' qr "Some text" > qr.png
```
