# KeyboardJYUT

KeyboardJYUT is a lightweight Android input method under active development.

The project starts from [Simple Keyboard](https://github.com/rkkr/simple-keyboard), which is itself based on AOSP LatinIME. The goal is to preserve that small, responsive keyboard architecture while adding multilingual composition and physical-keyboard support using a CedIME-style handler/composer/dictionary design.

## Current state

The repository is currently at the rebranding/baseline stage. The Android application ID is `jyut.keyboard`. Cantonese composition and the other planned input engines are not yet implemented in the main branch.

## Design goals

- Keep normal key handling lightweight and allocation-conscious.
- Support touch keyboards and physical keyboards as first-class input sources.
- Add Jyutping and Yale Cantonese input using a shared compact Cantonese dictionary.
- Support ten-key/T9 input across input methods, not only Latin or Cantonese.
- Add regional Stroke input with separate Hong Kong, Taiwan, Mainland and Japanese stroke data.
- Keep optional features such as handwriting, Japanese conversion, emoji, clipboard, translation and voice input lazy/on-demand so they do not slow ordinary typing.

## Upstream and licensing

KeyboardJYUT is derived from Simple Keyboard and AOSP LatinIME. Existing upstream copyright and Apache License 2.0 notices are retained in the source tree. See [LICENSE](LICENSE).

Additional dictionaries, language engines or optional modules may carry their own compatible licences and attribution; these will be documented when added.
