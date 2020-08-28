# remote-ssh-tunnel-controller-lib

## Dependencies:

*  python3
*  paramiko

## Usage example:

```bash
~$ git clone https://github.com/guallo/remote-ssh-tunnel-controller-lib.git controller_lib
~$ python3
>>> from controller_lib import factories
>>> ctl = factories.RSSHTControllerFactory.new()
>>> ctl.update()
>>> ctl.get_agents()
(<RSSHTAgent: raspberry>, <RSSHTAgent: agent-1>)
...
... # use ctl's object tree
...
>>> ctl.dispose()  # break cyclic references before ctl's deletion
```
