## DNS

In Cloudflare:

* A `CNAME` `homesecurity` points to `matthodge.github.io
* A page rule is configured to force `homesecurity.hodgkins.io/*` to always use HTTPS

## Deployment

Deployment happens with a push to `main` using GitHub Actions `.github/workflows/ci.yml` 

## Local Development

```bash
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
```