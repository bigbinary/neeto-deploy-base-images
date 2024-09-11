FROM ubuntu:24.04

RUN --mount=target=/build /build/setup.sh

# https://github.com/buildpacks/spec/blob/platform/0.13/platform.md#run-image
USER neetodeploy
LABEL io.buildpacks.base.distro.name="ubuntu"
LABEL io.buildpacks.base.distro.version="24.04"
LABEL io.buildpacks.base.homepage="https://github.com/heroku/base-images"
LABEL io.buildpacks.base.maintainer="Neetodeploy"

# Stack IDs are deprecated, but we still set this for backwards compatibility:
# https://github.com/buildpacks/spec/blob/platform/0.13/platform.md#iobuildpacksstack-labels
LABEL io.buildpacks.stack.id="heroku-24"
