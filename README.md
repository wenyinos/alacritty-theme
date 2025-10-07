# Alacritty Theme

Collection of colorschemes for easy configuration of the [Alacritty terminal
emulator].

## Installation

### Imports

Clone the repository, or download the theme of your choice:

```sh
# We use Alacritty's default Linux config directory as our storage location here.
mkdir -p ~/.config/alacritty/themes
git clone https://github.com/wenyinos/alacritty-theme ~/.config/alacritty/themes
cp ~/.config/alacritty/themes/alacritty.toml ~/.config/alacritty/
```

Add an import to your `alacritty.toml` (Replace `{theme}` with your desired
colorscheme):

```toml
[general]
import = [
    "~/.config/alacritty/themes/themes/{theme}.toml"
]
```

### Manual

To manually include a colorscheme in an existing `alacritty.toml`, you just need
to copy the entire content of the theme into the root level of your
configuration file.


## Contributing

Bug reports and pull requests are welcome on GitHub at the [alacritty-theme][alacritty-theme]
repository.

To add a new theme, please create a Pull Request. Note that submissions by theme
authors are not accepted, to ensure there's at least some community interest.
The following changes must be made for a new theme:

- Add your theme to the `themes` directory with the `{theme}.toml` file format
- Create a screenshot of your theme using the [`print_colors.sh`](./print_colors.sh) script
- Add the screenshot to the `images` directory with the `{theme}.png` file format
- Add your theme to the `README.md`, following alphabetical ordering

## Maintainers

* **indrajit** - *Author* - [eendroroy](https://github.com/eendroroy)
* **Christian Dürr** - *Maintainer* - [chrisduerr](https://github.com/chrisduerr)

## License

The project is available as open source under the terms of the [Apache License, Version 2.0](LICENSE)

[Alacritty terminal emulator]: https://github.com/alacritty/alacritty
[alacritty-theme]: https://github.com/alacritty/alacritty-theme
