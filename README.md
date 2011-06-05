An experimental fork of activewarehouse-etl (work in progress).

[![](http://travis-ci.org/thbar/tinytl.png)](http://travis-ci.org/#!/thbar/tinytl)

Mostly a "free thinking" experiment. There is no certainty I will keep working on this.

## Ideal goals

* should be compatible with
  * MRI 1.9.2
  * MRI 1.8.7
  * JRuby 1.6.2
  * Windows
* should be well-tested to make it easy to add/change/remove features
* should have tests that are dead-easy to run
* should have a core that is independent of ActiveRecord
* should have plugins for database-specific code
* should be documented from the code
* should have a command line binary
* should support bundler
* should largely use the syntax and transforms coming from aw-etl
* should support pre-post-load screens

* should run its tests in production
  * the rational behind this is that the etl can't be tested against all the databases and specific configurations (think: collations, encodings, os, bulk load behaviour), so at least one run should be done in production to check everything works as expected

* could support multi-core
* could support multi-agent

## Random thoughts

* not sure to use Cucumber or not
* having a well-bundled "upsert on unique keys" destination would be nice