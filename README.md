# Rails sample

## MEMO

### 1. Initial commit

### 2. Rails new

```sh
# Host
docker run -v $(pwd):/$(basename $(pwd)) -w /$(basename $(pwd)) -u $(id -u):$(id -g) --rm -it ruby:3.2.2-bookworm bash

# Docker
gem install rails
rails new . --skip-test --css tailwind

exit
```
