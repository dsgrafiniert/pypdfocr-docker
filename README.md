# pypdfocr-docker

PyPDFOCR on Docker

get rid of your paperwork...

## what is pypdfocr

PyPDFOCR converts a scanned PDF into an OCR'ed PDF using Tesseract-OCR and Ghostscript

- [https://pypi.python.org/pypi/pypdfocr/](https://pypi.python.org/pypi/pypdfocr/)
- [https://github.com/virantha/pypdfocr/](https://github.com/virantha/pypdfocr/)

## Dockerfile

[**Trusted Build**](https://hub.docker.com/r/dschoen/pypdfocr/)

This Docker image is based on the [official Ubuntu](https://hub.docker.com/_/ubuntu/) base image.

It incorporates a patch for issue [#41](https://github.com/virantha/pypdfocr/issues/41) of pypdfocr 0.9.0 likely to be fixed in 0.9.1

## How to use this image

```
docker run --rm dschoen/pypdfocr [-h] [-d] [-v] [-m] [-l LANG] [--preprocess]
                [--skip-preprocess] [-w WATCH_DIR] [-f] [-c CONFIGFILE] [-e]
                [-n]
                [pdf_filename]

```
docker run -v ~/Documents/Paper:/media dschoen/pypdfocr
```
For sample config see [config.yaml](https://github.com/mmatiaschek/pypdfocr-docker/blob/master/config.yaml) or pypdfocr authors repository [here](https://github.com/virantha/pypdfocr/).
