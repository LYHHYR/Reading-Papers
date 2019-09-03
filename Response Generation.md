## Response Generation by Context-aware Prototype Editing

edit-based > retrieval-based, generation-based

https://github.com/MarkWuNLP/ResponseEdit
dataset:{(context, response)}
(1) prototype selector: retrieval-based: prototypes response ~~safe responses~~, privacy issue
(2) context-aware neural editor

given a conversational context c
1) retrieve prototype: a similar context c' & its associated response r'
2) caculate an edit vector:
   insertion word embedding: words only in prototype
   deletion word embedding: words only in current context

conditional setting: the editor should consider the context (dialogue history) except in a response itself in the revision.
