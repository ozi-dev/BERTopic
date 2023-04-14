# BERTopic

BERTopic is an open-source project that implements the BERTopic algorithm, which is a topic modeling technique that uses pre-trained BERT models to generate embeddings for text data. This algorithm can be used to identify topics and subtopics within a large corpus of text data.

## Getting Started

To get started using BERTopic, first clone this repository to your local machine. You can do this by running the following command in your terminal:

```
git clone https://github.com/ozi-dev/BERTopic.git
```

Once you have the necessary dependencies installed, you can start using BERTopic. The `BERTopic.ipynb` notebook provides an example of how to use the algorithm.

## Usage

To use BERTopic, you can import the `BERTopic` class from the `bertopic` module:

```python
from bertopic import BERTopic
```

You can then create an instance of the `BERTopic` class and fit it on your data:

```python
model = BERTopic()
model.fit(data)
```

Once the model is trained, you can use the `transform` method to transform new documents into topic vectors:

```python
topic_vectors = model.transform(new_data)
```

You can also use the `get_topic` method to get the top N most representative documents for a given topic:

```python
representative_docs = model.get_topic(topic_id, n=10)
```

For more information on how to use BERTopic, please refer to the `BERTopic.ipynb` notebook.

## Contributing

If you would like to contribute to BERTopic, please feel free to submit a pull request with your changes. Before doing so, please make sure to run the unit tests using `pytest`.
