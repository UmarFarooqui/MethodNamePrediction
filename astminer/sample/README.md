### Method
As an example, consider the following method:

![Image description](images/method.jpg)

### Abstract syntax tree
The abstract syntax tree representation of the method is:

![Image description](images/ast.jpg)

### Token vocabulary
The token vocabulary emitted by the Astminer. Each token is associated with a unique token id.

![Image description](images/token_vocabulary.jpg)

### Node type vocabulary
The node type vocabulary emitted by the Astminer. Each node type along with a direction is associated with a unique node type id.

![Image description](images/node_type_vocabulary.jpg)

# Path vocabulary
The path vocabulary emitted by the Astminer. Paths are stored as sequences of node type ids.

![Image description](images/path_vocabulary.jpg)

# Path contexts
Path-contexts are encoded as (start token id, path id, end token id)

![Image description](images/path_context_encoded_form.jpg)