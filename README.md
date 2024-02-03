# make-it-black
This repo is just me Testing GH actions and how to do the referencing.   
This action is quite simple and just runs black and then commits the changes.

## Usage

```yaml
name: Make it black

on:
  push:
    branches:
      - main

jobs:
  make-it-black:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      - name: Make it black
        uses: GandalfsDad/make-it-black@v1
        with:
          python-version: '3.10'
```
