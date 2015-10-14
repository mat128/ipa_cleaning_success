What is that?
=============

This is a repository that simulates the Ironic-Python-Agent API. It simulates a cleaning success response.

Usage
-----

```
curl -v -X POST -H 'Content-Type: application/json' -d '{"agent_url": "https://raw.githubusercontent.com/mat128/ipa_cleaning_success/master/baremetal"}' http://ironic_host:6385/v1/nodes/NODE_UUID/vendor_passthru/heartbeat
```

You should be receiving a ```202 Accepted``` answer and the node should transition to ```AVAILABLE```.

Obviously, you should be knowing what you are doing to use that. This repository only serves as an easy way to serve this static json file.
