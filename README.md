# Singularity r-base

Singularity image for [R](https://www.r-project.org/) based on the [r-base](https://hub.docker.com/_/r-base/) docker image.

## Build

You can build a local Singularity image named `r-base.3.4.4.simg` with:

```
$ sudo -E singularity build --force r-base.3.4.4.simg Singularity
```

## Usage

Help

```console
$ singularity help r-base.3.4.4.simg


  R version 3.4.4 (2018-03-15) -- "Someone to Lean On"
  Copyright (C) 2018 The R Foundation for Statistical Computing
  Platform: x86_64-pc-linux-gnu (64-bit)

  Usage:
  $ singularity run r-base.3.4.4.simg [args]
  $ singularity run --app R r-base.3.4.4.simg [args]
  $ singularity run --app Rscript r-base.3.4.4.simg [args]
```

## Run

### R

The R command is launched using the default run command:

```bash
singularity run r-base.3.4.4.simg [args]
```

or as an explicit app:

```bash
singularity run --app R r-base.3.4.4.simg [args]
```

Example:

```console
$ singularity run --app R r-base.3.4.4.simg --version
R version 3.4.4 (2018-03-15) -- "Someone to Lean On"
Copyright (C) 2018 The R Foundation for Statistical Computing
Platform: x86_64-pc-linux-gnu (64-bit)

R is free software and comes with ABSOLUTELY NO WARRANTY.
You are welcome to redistribute it under the terms of the
GNU General Public License versions 2 or 3.
For more information about these matters see
http://www.gnu.org/licenses/.
```

### Rscript

The Rscript command is launched as an explicit app:

```bash
singularity run --app Rscript r-base.3.4.4.simg [args]
```

Example:

```console
$ singularity run --app Rscript r-base.3.4.4.simg --version
R scripting front-end version 3.4.4 (2018-03-15)
```

## Contributing

Bug reports and pull requests are welcome on GitHub at [https://github.com/mjstealey/r-base](https://github.com/mjstealey/r-base).

## License

The code is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
