# O.F - File Organizer
### [посмотри на русском](https://github.com/psdkiajhn/OF-Linux-Terminal-File-Organizer/blob/main/russian.md)
Do you have problem to organize your files❓ WITH O.F, NO MORE❗😃
Installtion is so easy, Even a Kid 🧒 can do it! You can see it from [here](https://github.com/psdkiajhn/OF-Linux-Terminal-File-Organizer/blob/main/README.md#installtion)
This app can oraganize your file in two was:
- Sorting by type (Lot's of extension type are built in, but you can add or change them😄)
- Sorting by extensions <br />
[Site](http://ofile.root.sx/) is update now! check it out


> [!NOTE]
> Python is needed, so install it

> [!TIP]
> Use sudo when you want to use `-a` or `-r` <br />
> if you see a sudo error without using any argument, it mean `file_types.json` in `/usr/OF/` is deleted, you must to use sudo to make it again <br />

> [!WARNING]
> "Please use sudo" 🟰 command need to change something in /usr/ folder and need sudo <br />
> "You can't use verbose and quiet together" 🟰 using `-v` and `-q` in the same command <br />
> "'/usr/OF/file_types.json' file has been deleted!" 🟰 type file has been deleted and OF must to make it again <br />
> "Needed file does not exist" 🟰 installtion files are deleted or have a problem, download again <br />

# Installtion

just install git and run these commands:
```

  git clone https://github.com/psdkiajhn/OF-Linux-Terminal-File-Organizer.git
  cd OF-Linux-Terminal-File-Organizer
  ./install

```
then it's in your terminal, enjoy❗😃

# Usage
after install, of command will add to your terminal <br />
you can use it with 10 argument or use it single:
```
  of -n | of --NO-NEW-FOLDER #*OF will not organize file with no Sorting Folder*
  of -h | of --help #*show help page*
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
This app make a Folder with a type or extension (`using -e or not`) to sort the files, but with this argument OF just sort files with existed folder, <br />
for e.g:
```
  before:       |    after:
  📁image       |    📁image (with test1.png and test2.jpg)
  🖼️test1.png   |    🎥test.mp4
  🖼️tset2.jpg   |
  🎥test.mp4    |
```
as you can `.mp4` file didn't organized because video folder doesn't exist❗ <br />
You can use it when you have our own sorted foldee but you add some new file, you can use `-n` or `--NO-NEW-FOLDER` to organize them with your old folder <br />

## Directory
if you want to organize a directory but your at another directory, <br />
you don't need to cd for going to that directory, just use `-d` or `--directory` like this: <br />
```
  of -d /usr/myfiles/
      or
  of -d="/usr/my\ files"
```

## Extension
if you want to sort your files using extention instead of their type, <br />
you can use `-e` or `--extension` <br />
This is an example: <br />
with -e: <br />
```
  before:       |    after:
  🖼️test1.png   |    📁png
  🖼️tset2.jpg   |    📁jpg
  🎥test.mp4    |    📁mp4
```
without -e: <br />
```
  before:       |    after:
  🖼️test1.png   |    📁image
  🖼️tset2.jpg   |    📁video
  🎥test.mp4    |
```

## Format
you want to see all supported extension❓ <br />
use `-f` or `--format` and just this <br />
You can also see all built-in supported format [here](https://github.com/psdkiajhn/OF-Linux-Terminal-File-Organizer/blob/main/README.md#Supported-extension) <br />

## Verbose & Quiet
if you want to know every thing use `-v` or `--verbose` <br />
and if you want to don't get any thing and just organize use `-q` or `--quiet` <br />

## Search
you don't know a extenstion is supported or not❓ <br />
just use `-s` or `--search`, message tell you every thing❗ <br />

## Add
you have a file with unsopported extension? <br />
just use `-a` or `--add` <br />
message will help you to add but I also help you here: <br />
for just one extenstion you can use `Extenstion:Type` <br />
and for several extenstion use `Extension1:Type, Extention2:Type2` <br />
for e.g: <br />
`psd:adobe photoshop, pdd:adobe photoshop` <br />
you change the built-in extenstion, like that: <br />
`png:custome, jpg:cutome` <br />

## Reset
if you don't want your changed extension or you accidentally broke them, <br />
No problem, just use `-r` or `--reset` and boom, your types have been reseted❗ <br />

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

# Uninstalltion

just run the uninstall file in app folder like this: <br />
```

  ./uninstall

```




















