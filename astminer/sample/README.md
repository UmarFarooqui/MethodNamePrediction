### Method
As an example, consider the following method:

![Image description](images/method.jpg)

### Abstract syntax tree
The abstract syntax tree representation of the method is generated using [1] and is shown below:

![Image description](images/ast.jpg)

### Token vocabulary
The token vocabulary emitted by the Astminer. Each token is associated with a unique token id.

![Image description](images/token_vocabulary.jpg)

### Node type vocabulary
The node type vocabulary emitted by the Astminer. Each node type along with a direction is associated with a unique node type id.

![Image description](images/node_type_vocabulary.jpg)

### Path vocabulary
The path vocabulary emitted by the Astminer. Paths are stored as sequences of node type ids.

![Image description](images/path_vocabulary.jpg)

### Path contexts
Path-contexts are encoded as (start token id, path id, end token id).

![Image description](images/path_context_encoded_form.jpg)

So, for the following abstract syntax tree path.

![Image description](images/ast_path_highlighted.jpg)

We are looking for the path-context having METHOD_NAME as the start token id and x as the end token id.

The path-context encoding is 9,30,2.

30 is the path id whose value is 32 27 28 3 4, where 32 is NAME UP, 27 is stmt|compound_stmt|funcdef UP, 28 is stmt|compound_stmt|funcdef DOWN, 3 is parameters DOWN and 4 is typedargslist|tfpdef|NAME DOWN.

References:
[1] https://ast-viewer.datacamp.com/editor