## [3.0.12](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.11...v3.0.12) (2023-01-11)


### Bug Fixes

* shrink configuration size ([d187ba1](https://github.com/EricCrosson/semantic-release-your-github-action/commit/d187ba1825f3ebcd99a6c4e45787903c48f10e96))

## [3.0.11](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.10...v3.0.11) (2023-01-10)


### Bug Fixes

* cache the correct path ([248e401](https://github.com/EricCrosson/semantic-release-your-github-action/commit/248e401a940b7af720821bbd9b5011a085bacd38))

## [3.0.10](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.9...v3.0.10) (2023-01-09)


### Bug Fixes

* use scratch workspace for temporary files ([162ec7f](https://github.com/EricCrosson/semantic-release-your-github-action/commit/162ec7f6713681ce369546d3481f7cd2801ffdae))

## [3.0.9](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.8...v3.0.9) (2023-01-08)


### Bug Fixes

* use install-github-release-binary ([f16d31c](https://github.com/EricCrosson/semantic-release-your-github-action/commit/f16d31ceef6fd8a94d0999bd7e8c9e0291d4856f))

## [3.0.8](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.7...v3.0.8) (2023-01-08)


### Bug Fixes

* Revert "fix: use install-github-release-binary" ([1e01856](https://github.com/EricCrosson/semantic-release-your-github-action/commit/1e018560a5270b7c54f0349e31a1d4084857e63e))
* use install-github-release-binary ([29f992c](https://github.com/EricCrosson/semantic-release-your-github-action/commit/29f992c1064e137dc5bf505736be9c03baa5e7ec))

## [3.0.8](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.7...v3.0.8) (2023-01-08)


### Bug Fixes

* use install-github-release-binary ([29f992c](https://github.com/EricCrosson/semantic-release-your-github-action/commit/29f992c1064e137dc5bf505736be9c03baa5e7ec))

## [3.0.7](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.6...v3.0.7) (2023-01-07)


### Bug Fixes

* restrict git assets to changelog ([7992cf7](https://github.com/EricCrosson/semantic-release-your-github-action/commit/7992cf74f0d91e360b46c4e0f746754b8bad0cdb))

## [3.0.6](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.5...v3.0.6) (2023-01-07)


### Bug Fixes

* correct copy/pasta in step name ([b9db974](https://github.com/EricCrosson/semantic-release-your-github-action/commit/b9db9744e084bf3d4fe93535bbaecc6582cc0988))

## [3.0.5](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.4...v3.0.5) (2023-01-06)


### Bug Fixes

* remove debug argument to semantic release ([aa0bfd2](https://github.com/EricCrosson/semantic-release-your-github-action/commit/aa0bfd28861b54e2a04d0d2d5f552438eee5eb14))

## [3.0.4](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.3...v3.0.4) (2023-01-06)


### Bug Fixes

* fall back to https repository URL ([41cc4ec](https://github.com/EricCrosson/semantic-release-your-github-action/commit/41cc4ecc0f0641c5db97c667984870a80740cf3d)), closes [#2](https://github.com/EricCrosson/semantic-release-your-github-action/issues/2)

## [3.0.3](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.2...v3.0.3) (2023-01-06)


### Bug Fixes

* add debug information while debugging semantic-release performance ([3bdd2a6](https://github.com/EricCrosson/semantic-release-your-github-action/commit/3bdd2a6ca41a6c850f2fc5b5d3fd22faa100d434))

## [3.0.2](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.1...v3.0.2) (2023-01-06)


### Bug Fixes

* only override package.json if using the actions semrel config ([f92a7ae](https://github.com/EricCrosson/semantic-release-your-github-action/commit/f92a7ae68bb88f5445cb9b2b0bd9f814413071d1))

## [3.0.1](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v3.0.0...v3.0.1) (2023-01-06)


### Bug Fixes

* use version number that exists ([ee42089](https://github.com/EricCrosson/semantic-release-your-github-action/commit/ee420890e533df075ad6a68f228550f7b0cfb7e1))

# [3.0.0](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v2.0.0...v3.0.0) (2023-01-06)


* feat!: auto detect and use the repository's semantic-release config ([e69137b](https://github.com/EricCrosson/semantic-release-your-github-action/commit/e69137bd468d68f59f015bc3e3ba44899d073904))


### BREAKING CHANGES

* the `config` input is no longer supported

# [2.0.0](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v1.0.3...v2.0.0) (2023-01-06)


* fix!: rename input to config ([e56f297](https://github.com/EricCrosson/semantic-release-your-github-action/commit/e56f297d84327465d3b5652329f1c772e5b593b1))


### BREAKING CHANGES

* rename `semantic-release-configuration` to `config`
for brevity.

## [1.0.3](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v1.0.2...v1.0.3) (2023-01-06)


### Bug Fixes

* specify repository url explicitly ([a200c6e](https://github.com/EricCrosson/semantic-release-your-github-action/commit/a200c6eaebee0a2c8e8971c0f8454062efb40ab3))

## [1.0.2](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v1.0.1...v1.0.2) (2023-01-06)


### Bug Fixes

* access content of downloaded file correctly ([e453fab](https://github.com/EricCrosson/semantic-release-your-github-action/commit/e453fab0caad9e3fd668358b1118574515568ea7))

## [1.0.1](https://github.com/EricCrosson/semantic-release-your-github-action/compare/v1.0.0...v1.0.1) (2023-01-06)


### Bug Fixes

* use correct path ([625f3c5](https://github.com/EricCrosson/semantic-release-your-github-action/commit/625f3c5daedaa1a33cd7fed2bd8276de979302e0))

# 1.0.0 (2023-01-06)


### Features

* initial commit ([c72c5f1](https://github.com/EricCrosson/semantic-release-your-github-action/commit/c72c5f13bd902b3e0e8de2071bb3b22f37a295a1))
