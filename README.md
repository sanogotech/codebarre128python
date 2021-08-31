# codebarre128python

The Best Python Packages for Generating Barcodes
treepoem is the most feature-rich Python package for rendering barcodes as images.

https://www.codeodis.com/content/24-polices-code-barre
Police Code Barre  en code barre ou par code python.

## Install
pip install treepoem

## CLI

treepoem --type code128 --output code128.png PyBay2018

treepoem --type qrcode --output qr.gif  https://jonasneubert.com/talks/pybay2018.html  eclevel=Q

##  Code Sample

```
import treepoem

img = treepoem.generate_barcode(
    barcode_type='qrcode',
    data='https://jonasneubert.com/talks/pybay2018.html',
    options={"eclevel": "Q"}
)
img.convert('1').save('qr.gif')


```

##  Code 128  example

![Code 128](https://github.com/sanogotech/codebarre128python/blob/main/code128.png "Code 128")
