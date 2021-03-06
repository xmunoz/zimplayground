# Solve Zimpl models with the SCIP solver via the browser

[![Go Report Card](https://goreportcard.com/badge/github.com/leethargo/zimplayground)](https://goreportcard.com/report/github.com/leethargo/zimplayground)

## Purpose
Inspired by the Go Playground, let users solve small Zimpl models
without the need to install anything. The models are solved on the
server with SCIP. The log output and solution values are provided to
the caller.

Results are also stored and can be shared between users via unique IDs
from hashes of the input data.

## Usage
```
$ ./zimplayground -h
Usage of ./zimplayground:
  -address=":8080": hostname:port of server
  -mem=100: SCIP memory limit (MB)
  -processes=4: limit on number of SCIP processes
  -scipExec="scip": (path to) scip executable
  -sleep=100: sleep before redirect to results (ms)
  -time=180: SCIP time limit (s)
```

## Dependencies
It is assumed that SCIP (with Zimpl) is installed on the server and
available in the =PATH= or explicitely specified as command-line flag.

See http://scip.zib.de for documentation on the installation process.

## Licensing
All of this code is MIT licensed. SCIP is available for academic use
under the "ZIB academic license".

