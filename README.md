# darklight
Simple cross-platform utility to output what appearance style is used.

You can use this like this in a shell script:

```zsh

if [[ "$(darklight)" == *"Dark"* ]]; then
  # handle dark
else
  # handle light
fi

```
