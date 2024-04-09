With the proliferation of vector-based methods in
modern information retrieval (IR) systems, there has been a
notable gap in providing explanations for retrieved documents,
thus fueling the need for explainable information retrieval
(XIR). While these methods demonstrate promising retrieval
performance, they often lack transparency in explaining why
certain documents are retrieved as query results. This paper
addresses this gap by proposing a comprehensive architecture
that integrates knowledge graphs into the XIR framework. Leveraging the structured information stored in knowledge graphs,
our approach aims to enhance the explainability of IR systems
at various stages of the retrieval process. Unlike existing XIR
approaches that primarily focus on refining the retrieval model,
our architecture emphasizes the utilization of existing knowledge
graphs to provide meaningful explanations for retrieval outcomes.
Through the incorporation of knowledge graphs, our proposed
framework seeks to bridge the gap between retrieval performance
and interpretability, thereby advancing the state-of-the-art in
explainable information retrieval.

Step by Step Implementation:
The methodology employed in this code begins with the
loading and preparation of the dataset extracted from the
provided CSV file.

Algorithm Steps:
1)Load dataset : Read the knowledge graph from the provided CSV file, assuming the format includes nodes representing documents and edges representing relationships between
documents.
2)Calculate Jaccard Similarity: Define a function Jaccard
similarity(query, document name) that calculates the Jaccard
similarity coefficient between the user query and the name of
each document in the knowledge graph. Jaccard similarity is
computed as the ratio of the size of the intersection of unique
tokens between the query and document name to the size of
their union.
3)Retrieve Top Related Documents: Iterate over each node
in the knowledge graph and calculate the Jaccard similarity
score between the user query and the name of each document.
Store the document name, similarity score, and URL (if
available) in a list of related documents. Sort the list of related
documents based on the similarity score in descending order to
obtain the top related documents. Return the top top n related
documents as the output.

