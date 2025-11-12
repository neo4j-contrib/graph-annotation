# graph-annotation

Conventions for annotating a graph, within the graph.

Annotations should be useful for:
- graph-level information
- describing labels and properties
- relating labels and properties
- enabling graphs to be self-documenting

This is similar to adding documentation to your source code through structured comments.

## Why? What problem does this solve?

There is often application-level knowledge about a graph that might be useful to others. Sometimes that
knowledge is added to the graph itself. 

For example, the [Knowledge Graph Builder](https://github.com/neo4j-labs/llm-graph-builder) 
creates a graph with some well-known labels:
- `__Entity__` labels for any extracted entity nodes
- `Document` and `Chunk` labels for parts of the lexical graph

Rather than being familiar with that tool's approach, it'd be great if the graph could
explain what labels exist and what they're used for. 

