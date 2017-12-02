# haskell-stack-travis-ci
Dead simple setup tools for running a Haskell build matrix using stack for several versions.

Scripts are adapted from those used for [haskell stack's build process](https://github.com/commercialhaskell/stack): 

To test builds for a Haskell project using [stack](https://github.com/commercialhaskell/stack): 

- `cp haskell-stack-travis-ci/.travis* my-project/`
- Optionally add/remove GHC version targets inside `.travis.yml`.
- For Libraries without binaries remove `BUILD_BINARY=1` from `.travis.yml` in the build matrix.
- ...?
- Profit

# Building and shipping binaries:
- Set the `BUILD_BINARY=1` environment variable for each variation in the build matrix you want to ship.
- Set a `GITHUB_TOKEN` environment variable for your project's builds in TravisCI; you can [create a token here](https://github.com/settings/tokens).
    - For a public repo select the `public_repo` scope
    - For a private repo select the `repo` scope
