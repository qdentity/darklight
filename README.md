# darklight

Simple cross-platform utility to output what appearance style is used.

Build the tool using `cargo build --release` and copy it into a location on your `$PATH` using `cp target/release/darklight /usr/local/bin/`.

An example of using this to set the theme of the [Helix](https://helix-editor.com) editor dynamically:

```zsh
if [[ "$(darklight)" == *"Dark"* ]]; then
    CATPPUCCINO="mocha"
else
    CATPPUCCINO="latte"
fi

CATPPUCCINO_TARGET="${HOME}/.config/helix/themes/catppuccin_${CATPPUCCINO}.toml"
CATPPUCCINO_LINK="${HOME}/.config/helix/themes/catppuccin.toml"

ln -sf $CATPPUCCINO_TARGET $CATPPUCCINO_LINK
```
