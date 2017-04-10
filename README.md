# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for Infrastructure Pip.Services

This is a workspace for [Infrastructure Pip.Services](https://github.com/pip-services-infra) 
implemented in 5 different languages: .NET, Java, Node.js, Go and Python.

The workspace enables build, test, and release across the following projects:

- **pip-services-devenv** - dockerized infrastructure services for development and testing
- **pip-services-logging-node** - Logging microservice in Node.js
- **pip-services-logging-python** - Logging microservice in Python
- **pip-clients-logging-node** - Client to Logging microservice in Node.js
- **pip-clients-logging-python** - Client to Logging microservice in Python
- **pip-services-counters-node** - Performance counters microservice in Node.js
- **pip-clients-counters-node** - Client to Performance counters microservice in Node.js
- **pip-services-eventlog-node** - System event log microservice in Node.js
- **pip-clients-eventlog-node** - Client to System event log microservice in Node.js
- **pip-services-statistics-node** - Statistics microservice in Node.js
- **pip-clients-statistics-node** - Client to Statistics microservice in Node.js

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services-infra/pip-services-infra-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop infrastructure services
```bash
> piptask start -component pip-services-devenv
> piptask stop -component pip-services-devenv
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The Infrastructure Pip.Services are created and maintained by **Sergey Seroukhov**
