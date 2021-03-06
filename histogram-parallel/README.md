# Parallel Histogram Example

In this example some random sample data is sent to the FPGA, it is then sorted into bins to create a histogram. The process of sorting the data has been parallelized to work efficiently on the FPGA.

## Structure

This directory contains code for an FPGA located at `main.go`. It also has a
command, `test-histogram` located at `cmd/test-histogram/main.go`

## Testing

To run this example in a simulator, execute the following:

```
reco test test-histogram
```

This will simulate the code running on an FPGA using a hardware simulator, and test it
using the `test-histogram` command.

## Building

```
reco build
```

This will build your commands and FPGA code for execution on hardware.
