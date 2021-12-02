# fluent-plugin-input-gelf

## Needed to fix miliseconds in order to get this outdated plugin to work:
- https://github.com/fotografde/fluent-plugin-input-gelf/commit/ad76e2a98832265aa59192329ec223f1f2f29abc

[![Build Status](https://travis-ci.org/MerlinDMC/fluent-plugin-input-gelf.svg?branch=master)](https://travis-ci.org/MerlinDMC/fluent-plugin-input-gelf)
[![Gem Version](https://badge.fury.io/rb/fluent-plugin-input-gelf.svg)](http://badge.fury.io/rb/fluent-plugin-input-gelf)

## Overview

A GELF compatible input for [Fluentd](http://www.fluentd.org/).

### Configuration

Accept GELF encoded messages over UDP

```
<source>
  type gelf
  tag example.gelf
  bind 127.0.0.1
  port 12201
</source>

<match example.gelf>
  type stdout
</match>
```
