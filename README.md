# go-exporter

Go-Tracer aims to instrument go-lang programs with Open Telemetry traces without visible code changes.

The go-tracer tool parses go program and insert the OTel exporting to all functions with the 1st parameter as a context. The exporter configurations are loaded from the environmental variables.

The target is to instrument below cases:

- Exported functions with context in args
- Http (and gRPC) clients

## Usage

The proposed way is to use `go build -a -toolexec` to rewrite the go code with AST utils.

## Development Phases

### Ph-1: Basic Instrument with AST

### Ph-2: Instrument with Dependencies
