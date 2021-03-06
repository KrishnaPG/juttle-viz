# Change Log

This file documents all notable changes to juttle-viz. The release numbering uses [semantic versioning](http://semver.org).

## 0.7.0

Released 2016-03-24

### Major Changes

- New highchart view [[#82](https://github.com/juttle/juttle-viz/pull/82)]
- juttle-view#consume_mark now expects object with time property [[#87](https://github.com/juttle/juttle-viz/pull/87)]

### Minor Changes

- Scatterchart no longer defaults title to 'name' field of points [[#85](https://github.com/juttle/juttle-viz/pull/85)]
- package.json: remove unused gulp-mocha-phantomjs dependency [[#81](https://github.com/juttle/juttle-viz/pull/81)]

### Bug Fixes

- Fix bug with scatterchart when 'name' was present in points but -title option wasn't specified [[#84](https://github.com/juttle/juttle-viz/issues/84)]

## 0.6.2

Release 2016-03-16

### Minor Changes

- table view: allow progressive option (so juttles written for CLI work here) [[#79](https://github.com/juttle/juttle-viz/pull/79)]

### Bug Fixes

- time-bars: properly handle case when hovering with no points present [[#77](https://github.com/juttle/juttle-viz/pull/77)]
- timechart: -interval creates break in line when it shouldn't [[#75](https://github.com/juttle/juttle-viz/issues/75)]

## 0.6.1

Released 2016-03-09

### Minor Changes

- timechart: support series 'width' option [[#72](https://github.com/juttle/juttle-viz/pull/72)]

### Bug Fixes

- Fix timechart bars width and positioning bug [[#71](https://github.com/juttle/juttle-viz/pull/71)]

## 0.6.0

Released 2016-03-09

### Major Changes

- Support markdown view for annotations [[#62](https://github.com/juttle/juttle-viz/issues/62)]

### Minor Changes

- timechart: use -interval value to set bar width when appropriate [[#64](https://github.com/juttle/juttle-viz/issues/64)]
- add ecosystem link [[#68](https://github.com/juttle/juttle-viz/pull/68)]
- text: make options and default behavior match CLI's `view text` [[#5]([https://github.com/juttle/juttle-viz/issues/5)]
 - default format to 'json' instead of raw
 - add support for `indent` option to control pretty-printing

### Bug Fixes

- json output of `view text` should be dense by default [[#5]([https://github.com/juttle/juttle-viz/issues/5)]

## 0.5.0

Released 2016-02-29

### Major Changes

- timechart: improve downsampling by changing option name from `-display.dataDensity` to `-downsample` and making it a `boolean` [[#6](https://github.com/juttle/juttle-viz/issues/6)]

## 0.4.3

Released 2016-02-22

### Bug Fixes

- juttle-view: remove drag icon from header [[#55](https://github.com/juttle/juttle-viz/pull/55)]
- bars.js: fix bug where sending a point with value 0 caused an exception [[#56](https://github.com/juttle/juttle-viz/pull/56)]

## 0.4.2

Released 2016-02-09

### Minor Changes

- change Outrigger references to Juttle Engine [[#49](https://github.com/juttle/juttle-viz/pull/49)]

## 0.4.1

Released 2016-02-08

### Minor Changes

- juttle-view: add static method getFlattenedParamValidationErrors [[#40](https://github.com/juttle/juttle-viz/pull/40)]

## 0.4.0

Released 2016-02-05

### Major Changes

- add umd build [[#43](https://github.com/juttle/juttle-viz/pull/43)]
 - This changes the location of the built css from `build/charts.css` to `dist/juttle-viz.css`

### Minor Changes

- timechart series detection: don't add fields with null values to a series' keys [[#44](https://github.com/juttle/juttle-viz/pull/44)]

## 0.3.1

Released 2016-01-21

### Bug Fixes

- time field: fix which views require time in points and which ones don't [[#32](https://github.com/juttle/juttle-viz/pull/32)]

## 0.3.0

Released 2016-01-20

### Major Changes

- Expect dates and durations [[#25](https://github.com/juttle/juttle-viz/pull/25)]
 - As part of this, make `moment` a peerDependency, change the example to use the `lib` build of juttle-viz, and remove the `dist` build. See PR for details.

## 0.2.0

Released 2016-01-06

### Major Changes

- barchart: move display.* params to top level [[#9](https://github.com/juttle/juttle-viz/pull/9)]
- Scatterchart remove display param nesting [[#10](https://github.com/juttle/juttle-viz/pull/10)]

## v0.1.0

Released 2015-12-18

### Major Changes

- Initial release of the standalone juttle-viz project.
