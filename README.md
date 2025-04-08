# update-gh-pages

This GitHub action update the `gh-pages` branch of a GAP package using
[GitHubPagesForGAP](https://github.com/gap-system/GitHubPagesForGAP)
whenever there is a new release. If everything is conf

## Usage

The action `update-gh-pages` has to be called by the workflow of a GAP
package.
It updates the package.


### Examples

See below for a minimal example to run this action.

#### Minimal example
```yaml
name: CI

on:
  push:
  pull_request:
  workflow_dispatch:

jobs:
  test:
    name: Test
    runs-on: ubuntu-latest

    steps:
      - uses: gap-actions/setup-gap@v2
      - uses: gap-actions/update-gh-pages@v1

```

## Contact
Please submit bug reports, suggestions for improvements and patches via
the [issue tracker](https://github.com/gap-actions/update-gh-pages/issues).

## License
The action `update-gh-pages` is free software; you can redistribute
and/or modify it under the terms of the GNU General Public License as published
by the Free Software Foundation; either version 2 of the License, or (at your
opinion) any later version. For details, see the file `LICENSE` distributed
with this action or the FSF's own site.
