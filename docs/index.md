# Getting Started

GenAI Impact is an open-source project built by [Data For Good](https://dataforgood.fr/) to highlight GenAI tools' energy consumption.

## Installation

```shell
pip install genai_impact
```


## Basic example for OpenAI

```python
from genai_impact import OpenAI

client = OpenAI()

response = client.chat.completions.create(
    model="gpt-3.5-turbo",
    messages=[
        {"role": "user", "content": "Hello World!"}
    ]
)

print(response.impacts)
```
