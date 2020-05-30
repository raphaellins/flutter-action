# Github Action for Flutter Build

This action provides `flutter` for Github Actions.

## How to use


`.github/workflows/main.yml`
```yml
on: push
name: build and test app
jobs:
  build:
    name: install dependencies
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v1

    - name: install dependencies
      uses: raphaellins/flutter-action@v1.0.0
      with:
        args: pub get
```
