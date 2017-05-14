pdftools

* install

```
sudo apt install ghostscript unoconv
```

**image to pdf**
```
unoconv -f pdf image.pdf
```

**word to pdf**
```
unoconv -f pdf file.docx
```

**pdf split**
```
yes | gs -sDEVICE=pdfwrite -dBATCH -o outname.%d.pdf input.pdf >& /dev/null
```

**pdf join**
```
gs -dBATCH -dNOPAUSE -q -sDEVICE=pdfwrite -sOutputFile=finished.pdffile1.pdf file2.pdf
```