# haskell-stack-travis-ci
Dead simple setup tools for running a Haskell build matrix using stack for several versions.

Scripts are adapted from those used for [haskell stack's build process](https://github.com/commercialhaskell/stack): 

To test builds for a Haskell project using [stack](https://github.com/commercialhaskell/stack): 

- Copy `.travis.yml` and `.travis-setup.sh` into the root of your repository
- Optionally add/remove GHC version targets inside `.travis.yml`.
- ...?
- Profit
