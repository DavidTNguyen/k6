TODO: Intro

## New Features!

### Category: Title (#533)

Description of feature.

**Docs**: [Title](http://k6.readme.io/docs/TODO)

## UX

* The consolidated user-supplied options (the final combination of config file options, exported script `options`, environment variables and command-line flags) are now exported back into the `options` script variable and can be accessed from the script. Thanks to @mohanprasaths for working on this! (#681 and #713)

## Bugs fixed!

* Logging: using the `--no-color` flag caused k6 to print output intended for `sdtout` to `stderr` instead. (#712)
* Logging: some error messages originating from Go's standard library did not obey the `--logformat` option. (#712)
* JSON output: when the standard output was used, the JSON collector closed it before k6 was finished printing the end-of-test summary to it (#715)
