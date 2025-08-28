# Legacy openGL bindings for OCaml

This is a fork of [lablgl](https://github.com/garrigue/lablgl) simply
stripped of TOGL and GLUT, and with an `opam` file (no other code modification).

The idea is to make maintenance easier with less dependencies.

It can be used as a pure library, and creating contexts can be done
with [tsdl](https://github.com/dbuenzli/tsdl) (the SDL2 bindings).

## Warning: old!

`lablgl` only binds very old openGL 1.x, and some of 2.0 (shaders). For more recent openGLs, see [tgls](https://github.com/dbuenzli/tgls)

# How to use this one instead of the original `lablgl`?

This library installs a package with the same name `lablgl` so it will
automatically override any previously reference to `lablgl`. Simply
do:

```
opam pin add https://github.com/sanette/lablgl-lib.git
opam install lablgl.1.07-lib
```

For instance, this allows you to install [oplot](https://github.com/sanette/oplot) with
```
opam install oplot
```

