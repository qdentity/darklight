# darklight

Simple cross-platform utility to output what appearance style is used.

Build the tool using `cargo build --release` and copy it into a location on your `$PATH` using `cp target/release/darklight /usr/local/bin/`.

Then you can use this like this in a shell script:

```zsh

if [[ "$(darklight)" == *"Dark"* ]]; then
  # handle dark
else
  # handle light
fi

```
