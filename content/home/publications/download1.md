+++
title = "ReliK"
file = "papers/ReliK.pdf"
weight = 1
+++

Can we assess a priori how well a knowledge graph embedding will
perform on a specific downstream task and in a specific part of the
knowledge graph? Knowledge graph embeddings (KGEs) repre-
sent entities (e.g., “da Vinci,” “Mona Lisa”) and relationships (e.g.,
“painted”) of a knowledge graph (KG) as vectors. KGEs are generated
by optimizing an embedding score, which assesses whether a triple
(e.g., “da Vinci,” “painted,” “Mona Lisa”) exists in the graph. KGEs
have been proven effective in a variety of web-related downstream
tasks, including, for instance, predicting relationships among en-
tities. However, the problem of anticipating the performance of a
given KGE in a certain downstream task and locally to a specific
individual triple, has not been tackled so far.
In this paper, we fill this gap with ReliK, a Reliability measure
for KGEs. ReliK relies solely on KGE embedding scores, is task- and
KGE-agnostic, and requires no further KGE training. As such, it is
particularly appealing for semantic web applications which call for
testing multiple KGE methods on various parts of the KG and on
each individual downstream task. Through extensive experiments,
we attest that ReliK correlates well with both common downstream
tasks, such as tail or relation prediction and triple classification,
as well as advanced downstream tasks, such as rule mining and
question answering, while preserving locality.