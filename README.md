# mgxs.co github actions

Scaffold for Github actions

## Setup
```yml
setup:
    name: setup
    runs-on: ubuntu-latest
    steps:
      - name: Checkout and Setup
        uses: mgxs-gnss/actions-setup@v1.3
        with: 
          artifact-name: 'build' # not required, won't create an artifact if not provided
          artifact-path: './build'  # not required, won't create an artifact if not provided
```

## Deploy 
### Usage

```yml
deploy:
    name: Deploy
    runs-on: ubuntu-latest
    steps:
      - name: Checkout and Setup
        uses: mgxs-gnss/actions-deploy@v1.3
        with: 
          artifact-name: 'build'
          artifact-path: './build'
          aws_access_key: ''
          aws_secret_key: ''
          aws_region: ''
          aws_s3_bucket: ''
          aws_cloudfront: '' # not required, if not provided, wont invalidate Cloudfront
```