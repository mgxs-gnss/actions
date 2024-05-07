# mgxs.co github action – Deploy

Scaffold for Github action node/ts/npm

## Usage

```yml
deploy:
    name: Deploy
    runs-on: ubuntu-latest
    steps:
      - name: Checkout and Setup
        uses: mgxs-gnss/actions-deploy@v1
        with: 
          artifact-name: 'build'
          artifact-path: './build'
          aws_access_key: ''
          aws_secret_key: ''
          aws_region: ''
          aws_s3_bucket: ''
          aws_cloudfront: '' # not required, if not provided, wont invalidate Cloudfront
```