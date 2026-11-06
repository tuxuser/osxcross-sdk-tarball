[![build](https://github.com/tuxuser/osxcross-sdk-tarball/actions/workflows/build.yml/badge.svg)](https://github.com/tuxuser/osxcross-sdk-tarball/actions/workflows/build.yml)

# osxcross-sdk-tarball

- You get macOS SDK tarballs that work with [osxcross](https://github.com/tpoechtrager/osxcross).
- We build them on macOS runners with the upstream packaging script.
- You download the tarball that matches your target SDK from releases.

## Usage

Download the tarball for your SDK from the releases page. Follow the osxcross docs to place it next to `build.sh`. Then run the osxcross build as usual.

## Releases

Releases are drafts. Each tag looks like `v15.5`. The tag matches the bundled SDK version. The version comes from the built filename. An example is `MacOSX15.5.sdk.tar.xz` for tag `v15.5`.

## Build

Push to `master` builds the SDK and uploads it as an artifact. Push a tag like `v15.5` to build and draft a release. You can also run the workflow by hand from the Actions tab. The SDK version is detected at build time. It depends on the Xcode version on the runner.
