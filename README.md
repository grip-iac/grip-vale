# grip-vale

This repository holds the Vale style for the Grip writing rules.

## Use the style

Add the package to `.vale.ini` in your repository:

```ini
StylesPath = .vale/styles
MinAlertLevel = suggestion
Packages = https://github.com/grip-iac/grip-vale/releases/download/v1.0.0/Grip.zip

[*.md]
BasedOnStyles = Grip
```

Run `vale sync`. Then run `vale docs/`. Add `.vale/styles/Grip/` to `.gitignore`.

## Release a new version

Push a tag that starts with `v`. The workflow in `.github/workflows/release.yml` builds `Grip.zip`
and attaches it to a GitHub release.
