# O.F - File Organizer For Linux

Do you have problem to organize your files❓ WITH O.F, NO MORE❗😃
Installtion is so easy, Even a Kid 🧒 can do it! You can see it from [here](https://github.com/psdkiajhn/OF-Linux-Terminal-File-Organizer/blob/main/README.md#installtion)
This app can oraganize your file in two was:
- Sorting by type (Lot's of extension type are built in, but you can add or change them😄)
- Sorting by extensions

> [!NOTE]
> Python is needed, so install it

> [!TIP]
> Use sudo when you want to add a new extension type

> [!IMPORTANT]
> U can make a folder with a type or extension of files you want to organize
> TO make other files untouched

# Usage
after install, of command will add to your terminal
you can use it with 10 argument or use it single:
```
  of -n | of --NO-NEW-FOLDER #*OF will not organize file with no Sorting Folder*
  of -h | of --help #*OF help page*
  of -d | of --directory #*Oraganizing another directory instead of current directory*
  of -v | of --verbose #*OF will say everything*
  of -q | of --quiet #*OF will don't say anything*
  of -f | of --format #*See all supported extension and their types*
  of -s | of --search #*Search in supported formats*
  of -a | of --add #*Add a new type for extension*
  of -r | of --reset #*reset all the custome types and extentions*
  of -e | of --extension #*OF will organize files by extension instead of their types!*
```
## No New Folder
This app make a Folder with a type or extension (`using -e or not`) to sort the files, but with this argument OF just sort files with existed folder,
for e.g:
```
  before:       |    after:
  📁image       |    📁image (with test1.png and test2.jpg)
  🖼️test1.png   |    🎥test.mp4
  🖼️tset2.jpg   |
  🎥test.mp4    |
```
as you can `.mp4` file didn't organized because video folder doesn't exist❗
You can use it when you have our own sorted foldee but you add some new file, you can use `-n` or `--NO-NEW-FOLDER` to organize them with your old folder

## Directory
if you want to organize a directory but your at another directory,
you don't need to cd for going to that directory, just use `-d` or `--directory` like this:
```
  of -d /usr/myfiles/
      or
  of -d="/usr/my\ files"
```

## Verbose & Quiet
if you want to know every thing use `-v` or `--verbose`
and if you want to don't get any thing and just organize use `-q` or `--quiet`

## Search
you don't know a extenstion is supported or not❓
just use `-s` or `--search`, message tell you every thing❗

## Format
you want to see all supported extension❓
use `-f` or `--format` and just this
You can also see all built-in supported format [here](https://github.com/psdkiajhn/OF-Linux-Terminal-File-Organizer/blob/main/README.md#Supported-extension)





# Supported extension
```
  bat -> executable
  exe -> executable
  msi -> executable
  sh -> executable
  vb -> executable
  vbs -> executable
  wsf -> executable
  apk -> executable
  ttf -> font
  otf -> font
  fnt -> font
  log -> text
  txt -> text
  tex -> text
  rtf -> text
  png -> image
  bmp -> image
  gif -> image
  ico -> image
  jpeg -> image
  svg -> image
  tif -> image
  scr -> image
  tiff -> image
  jpg -> image
  webp -> image
  mp4 -> video
  mkv -> video
  m4v -> video
  mpg -> video
  mpeg -> video
  mov -> video
  swf -> video
  vob -> video
  webm -> video
  wmv -> video
  mp3 -> audio
  aif -> audio
  cda -> audio
  mpa -> audio
  ogg -> audio
  wma -> audio
  wav -> audio
  bak -> backup
  cab -> windows
  cfg -> windows
  cur -> windows
  dll -> windows
  cpl -> windows
  drv -> windows
  dmp -> windows
  ini -> windows
  ink -> windows
  sys -> windows
  tmp -> windows
  icns -> mac
  7z -> copressed
  rar -> compressed
  zip -> compressed
  tar.gz -> compressed
  tgz -> compressed
  tbz -> compressed
  txz -> compressed
  tzst -> compressed
  tar.br -> compressed
  tar.bz2 -> compressed
  z -> compressed
  arj -> compressed
  tar.xz -> compressed
  tar.zst -> compressed
  deb -> package
  pkg -> package
  rpm -> package
  dmg -> disc image
  iso -> disc image
  toast -> disc image
  vcd -> disc image
  img -> disc image
  csv -> dataset
  dat -> dataset
  sql -> dataset
  db -> dataset
  dbf -> dataset
  mdb -> dataset
  sav -> dataset
  pdf -> document
  doc -> document
  wpd -> document
  docx -> document
  pptx -> document
  ppt -> document
  pps -> document
  odp -> document
  xls -> document
  xlsm -> document
  xlsx -> document
  xml -> programing
  py -> programing
  cpp -> programing
  java -> programing
  go -> programing
  html -> programing
  css -> programing
  cs -> programing
  js -> programing
  jsp -> programing
  php -> programing
  htm -> programing
  xhtml -> programing
  jar -> programing
  c -> programing
  class -> programing
  h -> programing
  cgi -> programing
  pl -> programing
  swift -> programing
```


# Installtion

just install git and run these commands:
```

  git clone https://github.com/psdkiajhn/OF-Linux-Terminal-File-Organizer.git
  cd OF-Linux-Terminal-File-Organizer
  ./install

```
then it's in your terminal, enjoy❗😃

# Uninstalltion

just run the uninstall file in app folder like this:
```

  ./uninstall

```




















