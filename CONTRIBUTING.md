# Contributing to Afterhall

Thank you for your interest! Afterhall is still in early development, so contribution processes may change.

## Ground rules

- **Code, documentation and the format specification are written in English.** The user interface and interviews start in German, and translations are welcome.
- **Configuration instead of hard-coded values.** Groups, people, backup targets, models and languages must be configurable.
- **Safe defaults are not optional.** New entries default to "only me". Legacy answers need sources. The likeness notice and third-party protection must never be removable through configuration.
- **Never use real personal data** in issues, tests, fixtures or screenshots. Use invented data.

## Importers

Importers (WhatsApp, Telegram, Facebook, …) are the easiest way to contribute. Every importer must:

1. leave the original export untouched
2. write records in the current format version (JSON Lines)
3. set `author` correctly so that the user's own messages are separated from other people's
4. set `source_file` so every record points back to its original file
5. ship with anonymised sample data for its tests

## Workflow

1. For anything larger than a typo, please open an issue first.
2. Fork the repository and create a branch (`feat/…`, `fix/…`, `importer/…`).
3. Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages.
4. Open a pull request. `main` is protected and needs a review.

## License

By contributing, you agree that your contribution is licensed under the license of the respective repository (AGPL-3.0 for code, CC-BY-4.0 for the format specification).

## Security

Please do not report security problems as issues. See [SECURITY.md](SECURITY.md).
