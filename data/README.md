The data is downloaded from https://s3.amazonaws.com/code-search-net/CodeSearchNet/v2/python.zip

Data is stored in jsonlines format. Each line in the uncompressed file represents one example (usually a function with an associated comment).

repo: the owner/repo

path: the full path to the original file

func_name: the function or method name

original_string: the raw string before tokenization or parsing

language: the programming language

code: the part of the original_string that is code

code_tokens: tokenized version of code

docstring: the top-level comment or docstring, if it exists in the original string

docstring_tokens: tokenized version of docstring

sha: this field is not being used

partition: a flag indicating what partition this datum belongs to of {train, valid, test, etc.} This is not used by the model. Instead we rely on directory structure to denote the partition of the data

url: the url for the code snippet including the line numbers

The data is from 13590 python repos. The total samples i.e the code, func_name etc points are 457461. We will increase our dataset, if need arises, by exploring other public python repositories and datasets.

References:

https://github.com/github/CodeSearchNet