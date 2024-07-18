# LLM Flow

**LLM Flow** is a Large Language Model Work Flow Framework.

## Basic Construction

The fundamental construction for the LLM Flow is a direct graph (no need for the graph to be a DAG), in Computer Science.

### Node

A node is something that receives an input: a string(In some particular case, the node can take nothing) and returns an output: also a string(In some particular case, the node can give nothing), will be either passed to another node, or directly shows to user.

There is some pre-defined node types to make development easier.

### Edge

Edge is consider to be the `pass` process mentioned in the `Node` part. Which means that neither the developer nor the user need to consider about it.

## Different Types of Node

### Node Base

This is the base class of every node type, it is more like a interface, though it can return what it receives.

### LLM Node Base

This is the base class of every node type that needs to interact with LLM.

### Inputter

An `Inputter` takes the user input(for developer, it takes nothing) and directly returns it.

### Outputter

An `Outputter` takes a string and directly shows it to user(for developer, it returns nothing).

### Extractor

An `Extractor` takes a string, extracts informations out of it, structures it and returns it.
