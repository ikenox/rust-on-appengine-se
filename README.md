# Rust Sample App on Google App Engine Standard Environment


## Requirements

- Docker
- gcloud command-line tool

## Build and Deploy

```sh
# Build native binary for App Engine
docker run \
     --rm \
     --interactive \
     --tty \
     --volume (pwd):/opt/volume \
     --workdir /opt/volume \
     amd64/rust cargo build --release

# Deploy to App Engine
gcloud app deploy --project=your-gcp-project-id --version=sample
```
