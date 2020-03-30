# calcium
Scripts used for preprocessing images of Ca2+ signal during Xenopus neural tube formation. These are associated with the following publication: Makoto Suzuki, Masanao Sato, Hiroshi Koyama, Yusuke Hara, Kentaro Hayashi, Naoko Yasue, Hiromi Imamura, Toshihiko Fujimori, Takeharu Nagai, Robert E. Campbell, Naoto Ueno. Development 2017 144: 1307-1316; doi: 10.1242/dev.141952.
https://dev.biologists.org/content/144/7/1307.

## Usage
```
perl Ca_imaging_preprocessing.v1.4_short3g.pl path_to_base_dir
```
`Ca_imaging_preprocessing.v1.4_short3g.pl` is basically a script organizing the preprocessing pipeline with other scripts.

Under the directory which path is `path_to_base_dir`, there must be following files and directories:
- GFP multitiff file
- R-GECO multitiff file
- a directory containing single tiff files generated from the GFP multitiff
- a directory containing single tiff files generated from the R-GECO multitiff

__Note__ that strings used in pattern matching such as w0000 are set for our file naming convensions. Change the strings for other file naming convensions.

## Input files/directories
- GFP multitiff file
- R-GECO multitiff file
- a directory containing single tiff files generated from the GFP multitiff
- a directory containing single tiff files generated from the R-GECO multitiff

## Output file
- Normalized R-GECO image file (.tiff)(from `R-GECO_local_normalization_g.R`)

