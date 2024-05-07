# mgxs.co github action

Scaffold for Github action node/ts/npm

## Usage

```yml
setup:
    name: setup
    runs-on: ubuntu-latest
    steps:
      - name: Checkout and Setup
        uses: mgxs-gnss/actions-setup@v1
        with: 
          artifact-name: 'build' # not required, won't create an artifact if not provided
          artifact-path: './build'  # not required, won't create an artifact if not provided
```