bbdoc
=====

Bob Buzzard&#39;s Salesforce CLI Plugin to allow documentation to be autogenerated from org metadata.

[![Version](https://img.shields.io/npm/v/bbdoc.svg)](https://npmjs.org/package/bbdoc)
[![Downloads/week](https://img.shields.io/npm/dw/bbdoc.svg)](https://npmjs.org/package/bbdoc)
[![License](https://img.shields.io/npm/l/bbdoc.svg)](https://github.com/keirbowden/LDNSCall2020Plugin/blob/master/package.json)


```sh-session
INSTALLING
  $ sfdx plugins:install bbdoc
  $ sfdx plugins
    @salesforce/sfdx-diff 0.0.6
       ...
    bbdoc 3.4.6

USAGE
  $ sfdx bbdoc:doc -r <string> -s <string> [-c <string>] [--json] [--loglevel 
  trace|debug|info|warn|error|fatal|TRACE|DEBUG|INFO|WARN|ERROR|FATAL]

OPTIONS
  -c, --config=config                                                               configuration file

  -r, --report-dir=report-dir                                                       (required) directory to store the
                                                                                    generated report

  -s, --source-dir=source-dir                                                       (required) source directory
                                                                                    containing the org metadata

  --json                                                                            format output as json

  --loglevel=(trace|debug|info|warn|error|fatal|TRACE|DEBUG|INFO|WARN|ERROR|FATAL)  [default: warn] logging level for
                                                                                    this command invocation

EXAMPLE
  $ sfdx bbdoc:doc --config ./config/bbdoc-config.json --report-dir ./report --source-dir force-app/main/default/
  Documenting Org
  Documented Org
  Report generated at report/index.html
```

_See code: [src/commands/bbdoc/doc.ts](https://github.com/keirbowden/LDNSCall2020Plugin/blob/V3.4.0/src/commands/bbdoc/doc.ts)_

For more information, including how to configure the plug-in for a specific codebase, see the [Org Documentor Documented](https://sites.google.com/view/orgdocumentor)
