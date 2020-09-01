# remote-ssh-tunnel-controller-lib

```shell
pip install remote-ssh-tunnel-controller-lib
```

```python3
>>> from rssht_controller_lib import factories
>>> ctl = factories.RSSHTControllerFactory.new()
>>> ctl.update()
>>> ctl.get_agents()
(<RSSHTAgent: raspberry-pi-1>, <RSSHTAgent: other-agent>)
...
... # use ctl's object tree
...
>>> ctl.dispose()  # break cyclic references before ctl's deletion
```
