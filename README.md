# Rust Sample App on Google App Engine Standard Environment


## Requirements

- Docker
- gcloud command-line tool

## Build

```sh
docker run \
     --rm \
     --interactive \
     --tty \
     --volume (pwd):/opt/volume \
     --workdir /opt/volume \
     amd64/rust cargo build --release
```

## Deploy

```sh
gcloud app deploy --project=your-gcp-project-id --version=rust-sample
```
