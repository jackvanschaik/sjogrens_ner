# sjogrens_ner
Inducing a Sjogren's Syndrome Knowledge Graph From Medical Literature Using Transfer Learning

## df_all_sjogrens_entities.csv

This CSV contains all mined relationships between normalized entities. The columns are as follows:

* __sent_id__: A unique sentence id 
* __sent__: The original source sentence, mined from PubMed and classified as causal
* __phrase_id__: A unique phrase id within each sentence
* __phrase__: The phrase in the __sent__ tagged identified by the ELECTRA model
* __phrase_span__: The character span of __phrase__ in __sent__
* __entity_id__: Unique cause/effect entity id within each phrase
* __entity__: A named entity identified by the pretrained sciSpacy model
* __CE__: Inidicator if the entity was labelled as "cause" or "effect" by the ELECTRA model
* __label__: The entity label from the sciSpacy model
