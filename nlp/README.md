# Hugging Face
## Convert TF to Torch
```
from transformers import AutoTokenizer, AutoModel

tokenizer = AutoTokenizer.from_pretrained("tf_model")
model = AutoModel.from_pretrained("tf_model", from_tf=True)

model.save_pretrained("torch_model")
```
