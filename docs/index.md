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

## Logging into Kodexa

The first thing you need to do is log into a Kodexa platform instance. You can do this by running the `login` command:

```shell
$ kodexa login
```

You will need to provide the URL of the Kodexa platform instance you want to log into. You can also provide the email
and password for the Kodexa platform instance.

Once you have successfully logged in you can see the details of the Kodexa platform instance you are logged into by
running the `platform` command:

```shell
$ kodexa platform
```

Your personal API token will be stored in your home directory, based on your operating system it will be:

* **macOS** ~/Library/Application Support/kodexa-cli
* **Linux** ~/.local/share/kodexa-cli
* **Windows** C:\Documents and Settings\{User}\Application Data\Local Settings\kodexa\kodexa-cli
or C:\Documents and Settings\{User}\Application Data\kodexa\kodexa-cli

This file is used to authenticate you to the Kodexa platform instance. You can also provide the API token as an
environment variable called `KODEXA_ACCESS_TOKEN`.
