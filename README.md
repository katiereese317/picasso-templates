# Picasso templates

This repository holds [picasso](https://github.com/eveld/picasso) templates that can be used to generate image assets.

Picasso is a tool that can take a template and data, and generate images from them. The templates that Picasso uses are written in HCL (HashiCorp Configuration Language) and define the input, output and design of the resulting image.

Some of these templates might require additional assets to be copied into this repository for them to work.
Due to licenses for those assets, they are not included in this repository.

The paths in the templates are computed from the directory the binary is run in.
This means that a template that refers to `images/background.png` and is executed with the command `picasso generate -t hashitalks/regional/banner.hcl` will look for the background at `$PWD/images/background.png`.
