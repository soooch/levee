
# [levee]

levee is a statusbar for the [river] wayland compositor, written in [zig]
without any UI toolkit. It currently provides full support for workspace tags
and displays battery capacity and screen brightness.

Some important things are not implemented yet:

* configuration via cli flags
* configuration via config file

## Build

```
git clone --recurse-submodules https://git.sr.ht/~andreafeletto/levee
cd levee
zig build -Drelease-safe --prefix ~/.local install
```

## Usage

Add the following toward the end of `$XDG_CONFIG_HOME/river/init`:

```
riverctl spawn levee
```

## Dependencies

* [zig] 0.9.0
* [wayland] 1.20.0
* [pixman] 0.40.0
* [fcft] 3.0.1

## Contributing

You are welcome to send patches to the [mailing list] or report bugs on the
[issue tracker].

If you aren't familiar with `git send-email`, you can use the [web interface]
or learn about it following this excellent [tutorial].

[levee]: https://sr.ht/~andreafeletto/levee
[river]: https://github.com/riverwm/river/
[zig]: https://ziglang.org/
[wayland]: https://wayland.freedesktop.org/
[pixman]: http://pixman.org/
[fcft]: https://codeberg.org/dnkl/fcft/
[mailing list]: https://lists.sr.ht/~andreafeletto/public-inbox
[issue tracker]: https://todo.sr.ht/~andreafeletto/levee
[web interface]: https://git.sr.ht/~andreafeletto/levee/send-email
[tutorial]: https://git-send-email.io
