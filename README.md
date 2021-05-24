# A minimal Jekyll Docker ARM64 image
[![[builder] CI for releases](https://github.com/mrxder/jekyll-docker-arm64/actions/workflows/build_deploy.yml/badge.svg)](https://github.com/mrxder/jekyll-docker-arm64/actions/workflows/build_deploy.yml)
---
This Docker image/file can be used for development on ARM64 based machines like Macs based on Apple Silicon like the M1 chip.

# Jekyll Build
```
docker run --rm -v "$PWD:/var/jekyll" -it mrxder/jekyll-docker-arm64:latest jekyll build
```

# Jekyll Serve (Develop)
```
docker run --rm -v "$PWD:/var/jekyll" -p 4000:4000 -it mrxder/jekyll-docker-arm64:latest jekyll serve --host=0.0.0.0
```

# Build Docker image
```
docker build --tag mrxder/jekyll-docker-arm64:latest ./docker
```