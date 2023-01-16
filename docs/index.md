Kodexa command line tools provide an easy way to work with a Kodexa platform instance from the command line. The tools
are built on top of the Python SDK and provide a simple way to interact with the platform.

## Installation

The Kodexa command line tools are available on PyPi and can be installed with pip:

```shell
$ pip install kodexa-cli
```

## Usage

The Kodexa command line tools are available as a single command called `kodexa`. You can see the available commands by
running `kodexa --help`:

```shell
$ kodexa --help
Usage: kodexa [OPTIONS] COMMAND [ARGS]...

Options:
  -v, --verbose  Enable verbose output.
  --help         Show this message and exit.

Commands:
  delete          Delete the given resource (based on ref)
  deploy          Deploy a component to a Kodexa platform instance from a...
  document
  export-project
  get             List the instance of the object type
  import-project
  login           Logs into the specified platform environment using the...
  logs            Get logs for an execution
  package         Package an extension pack based on the kodexa.yml file
  platform        Get the details for the Kodexa instance we are logged into
  project         Get all the details for a specific project
  query           Query the documents in a given document store
  send-event      Send an event to an assistant
  upload          Upload the contents of a file or directory to a Kodexa...
  version
```
    