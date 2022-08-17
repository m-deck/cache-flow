[![CircleCI](https://circleci.com/gh/spectacles-ci/spectacles.svg?style=svg)](https://circleci.com/gh/spectacles-ci/spectacles)
[![codecov](https://codecov.io/gh/spectacles-ci/spectacles/branch/master/graph/badge.svg)](https://codecov.io/gh/spectacles-ci/spectacles)
[![downloads](https://img.shields.io/pypi/dm/spectacles)](https://img.shields.io/pypi/dm/spectacles)

## What is Cache Flow?

**Cache Flow is a command-line, cache management tool for Looker and LookML.** Cache Flow "pre-warms" your Looker cache for specified dashboard IDs. Currently, for the first Looker user who runs a dashboard after a cache reset, they will have to wait for the entire dashboard to load from SQL, resulting in a slow experience. Subsequent users (who load the dashboard before the cache resets again) will experience quick load times as the dashboard will load instantly from Looker's cache.

Cache Flow aims to solve the first-user problem by **being** that first user so that all your real users can benefit from the quick load-from-cache times when possible.

Cache Flow is forked from Spectacles, another favorite Looker tool of ours, as we wanted to borrow the concurrency management functionality instead of reinventing the wheel ourselves. Cache Flow is not intended to perform any sort of validation that Spectacles does. Currently there is a lot of leftover code from Spectacles left in this repository - cleanup is in progress.

## Documentation

TBA

## Installation

TBA

## Why we built this

Looker's caching functionality is great, but there is currently no easy way to pre-warm Looker's cache for a list of dashboards on a regular basis without creating individual schedules to run those dashboards. Cache Flow allows administrators or developers to specify a list of dashboards across the whole instance and schedule them to run in sequence, with specified concurrency limits so as not to cause too much traffic.

## Community

TBA
