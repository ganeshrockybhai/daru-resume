# Daru Resume

This is a resume render for Daru custom design using hackmyresume

## Installation

Install prerequisite hackmyresume 

```
npm install hackmyresume -g
```

## Usage

```
#Installing jsonresume-theme-daru-new nom package
npm i jsonresume-theme-daru-new

##Generate resume
hackmyresume build resume.json TO out/resume.all -t node_modules/jsonresume-theme-daru
```
## For Generating Pdf with header/footer
```
#Install wkhtmltopdf
wget https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6-1/wkhtmltox_0.12.6-1.focal_amd64.deb
sudo dpkg -i wkhtmltox_0.12.6-1.focal_amd64.deb

#To Generate pdf
wkhtmltopdf --margin-left '0mm' --margin-right '0mm' --header-html ./header.html --footer-html ./footer.html ./out/resume.pdf.html ./resumefinal.pdf

#Note
Sample header.html and footer.html can be found in GitHub repo.
```