# orm_llm_notebooks
Encoder and decoder models using Huggingface transformers

Contains project files for Token classfications (NER), MultiClass Classification for BERT Encoder architecture and Decoder architecture using Llama 3 

For NER, product titles were tokenized and a BERT model was trained using manually labeled grocery data to classify tokens according to serveral common grocery categories such as Flavour, Milk Fat % and Product type

For MultiClass classfication, products were trained on data scraped from the Metro Website, with their category data such as Dairy and Eggs, Produce etc.
Inference allows you to take a product title and determine the best categorical fit using the Metro classfication system.

For The Decoder Architecture, the Llama 3 model was trained using peft and qLoRA. The process finetued the model to generate the best category given an input of a product title.