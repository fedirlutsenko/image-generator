# Twitter Card Image Generator

Generate Twitter card image for your blog posts.

![sample](./example/blog-post2.png)

## Installation

```
go get github.com/Ladicle/tcardgen
```

## Usage

```
$ tcardgen -h
Generate TwitterCard(OGP) images for your Hugo posts.
Supported front-matters are title, author, categories, tags, and date.

Usage:
  tcardgen [-f <FONTDIR>] [-o <OUTDIR>] [-t <TEMPLATE>] <FILE>...

Examples:
# Generate a image and output to the example directory.
tcardgen --fontDir=font --outDir=example --template=example/template.png example/blog-post.md

# Generate multiple images.
tcardgen --template=example/template.png example/*.md

Flags:
  -f, --fontDir string    Set a font directory. (default "font")
  -h, --help              help for tcardgen
  -o, --outDir string     Set an output directory. (default "out")
  -t, --template string   Set a template image file. (default "template.png")
```
