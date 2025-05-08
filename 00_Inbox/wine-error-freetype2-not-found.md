
## wine-error-freetype2-not-found

**tags:** #type/log #topic/error 

### Catatan
Saat saya mau menginstall winetricks `vcrun2019`, floating window dari instalasi vcrun2019 malah hitam, dan muncul error

```bash

Wine cannot find the FreeType font library.  To enable Wine to
use TrueType fonts please install a version of FreeType greater than
or equal to 2.0.5.
http://www.freetype.org
Wine cannot find the FreeType font library.  To enable Wine to
use TrueType fonts please install a version of FreeType greater than
or equal to 2.0.5.
http://www.freetype.org

```

Hal yang harus dilakukan adalah menginstal freetype2 agar floating windownya tidak hitam, untuk menginstallnya bisa dengan

```bash
sudo pacman -S lib32-freetype2
```

