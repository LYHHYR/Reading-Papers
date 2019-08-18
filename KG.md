# Knowledge Graph

### *1. Barack’s Wife Hillary:Using Knowledge Graphs for Fact-Aware Language Modeling*
https://arxiv.org/abs/1906.07241

#### *data set:* Linked WikiText-2
https://rloganiv.github.io/linked-wikitext-2/#/

#### *compared against:* AWD-LSTM
###### language models:  

   p(xt|x<t)
   
   xt -- the next token which is going to be predicted
   
   x<t -- the sequence have already been known

###### RNN language models: 

   p(xt|x<t) = softmax(Wh*ht + b),
   
   ht = RNN(ht−1, xt−1)

#### *knowledge graph language model* **(KGLM)**

   a dynamically growing *local knowledge graph* = {entities that have already been mentioned} 

   1) render a new entity, growing the local knowledge graph
   
   2) render a fact from local graph

###### notations
   nodes: entities E
   
   edges: relations R
   
   KG = {(p,r,e)| p ∈ E , r ∈ R, e ∈ E}
   
   p: a parent entity


p(xt,Et|x<t,E<t)


