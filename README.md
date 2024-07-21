# haskell-github-release-test

This is a project to test the semi-automatic creation of github releases for a stack-based Haskell project.
The idea is to:

* Build and test the project on every commit on any branch
* when a tag is pushed that starts with `v`, create a release
  * The release should be a draft release
  * The release should contain artifacts for the built executable on different platforms
  * For each platform, after uploading the release artifact, download it and see if it works (basically something like a smoke test)
