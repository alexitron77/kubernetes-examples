## Node affinity

- [node-affinity](scripts/node-affinity.yaml)

You may need to deploy your pods on specific node. This can be related to resources (cpu/memory), hardware or whatever reasons.
Node affinity is a property that is added at the container level to specify which node it has to run inside. Basically, the node is targeted based on the label previouslyadded.

Use the command `kubectl label nodes <nodename> disk=ssd` to label the node with the attribute "disk"

