# Dash Documentation for Claris/FileMaker

- [Jason P. Scharf](https://github.com/iNtergrated/) [@jpscharf](https://twitter.com/jpscharf) & others.

## Docset Generation

- Clone the this [repository](git@github.com:petrowsky/FileMaker-Dash-Docset.git):

  > `git clone git@github.com:petrowsky/FileMaker-Dash-Docset.git`

- Download the FileMaker Help File -> [Claris support page](https://support.claris.com/s/article/Claris-FileMaker-19-Documentation-Releases-Notes-and-FileMaker-Help?language=en_US) or...

  > `curl https://help.claris.com/downloads/fmp-19-help-en.zip -O`

- Extract the zip file, rename the folder to **FileMaker Help**, and copy to the root of this folder.

  > ```
  > unzip fmp-19-help-en.zip
  > mv en "FileMaker Help"
  > ```

- Install dependencies: `composer install` (need composer [on a Mac](https://brew.sh)?, [on Windows](https://getcomposer.org/doc/00-intro.md)?)

- Generate the docset using: `php generate`

- The generated docset can be found inside the build folder: **`build/FileMaker.docset`**
