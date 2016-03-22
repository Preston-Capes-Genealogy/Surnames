# Surnames
Word files containing genealogical information for Preston Capes residents.

The data files contained in this repository have been converted to PDF and put
on the website: [www.prestoncapes-genealogy.org](http://www.prestoncapes-genealogy.org)

## Convert to PDF
To convert the Word documents to PDF I used this command (on my Mac)

```bash
for F in *.doc; do 
  curl --progress-bar -F inputDocument=@"$F" \
    http://www.doc2pdf.net/convert/document.pdf > "${F/doc/pdf}"; 
done
```
