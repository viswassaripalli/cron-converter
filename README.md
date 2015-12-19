# cron-converter

Cron string parser for node

[![Build Status](https://travis-ci.org/roccivic/cron-converter.svg)](https://travis-ci.org/roccivic/cron-converter)
[![Coverage Status](https://coveralls.io/repos/roccivic/cron-converter/badge.svg?branch=master&service=github)](https://coveralls.io/github/roccivic/cron-converter?branch=master)
[![Dependency Status](https://david-dm.org/roccivic/cron-converter.svg)](https://david-dm.org/roccivic/cron-converter)
[![devDependency Status](https://david-dm.org/roccivic/cron-converter/dev-status.svg)](https://david-dm.org/roccivic/cron-converter#info=devDependencies)
[![Code Climate](https://codeclimate.com/github/roccivic/cron-converter/badges/gpa.svg)](https://codeclimate.com/github/roccivic/cron-converter)
[![Issue Count](https://codeclimate.com/github/roccivic/cron-converter/badges/issue_count.svg)](https://codeclimate.com/github/roccivic/cron-converter)
[![MIT License Badge](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/roccivic/cron-converter/blob/master/LICENCE.txt)

## Install

```
npm install
```

## Lint

```
gulp lint
```

## Test

```
gulp test
```

## Use

```js
// Get the Cron constructor
var Cron = require('cron');

// Create a new instance
var cronInstance = new Cron();

// Parse a cron string
cronInstance.parse('1 1 1 1 1');

// Prints: [ [1], [1], [1], [1], [1] ]
console.log(cronInstance.toArray());

// Prints: '1 1 1 1 1'
console.log(cronInstance.toString());

```