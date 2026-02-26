# finetune-llama3.2
Finetuning LLaMA 3.2 model using QLoRA to predict product price based on description. Data preparation and model evaluation against business objectives.

Key components 
- Finetuning datasets generation ( https://huggingface.co/datasets/abdelkader/items_prompts_full/) 

- Evaluating the base model (without finetuning)
- Setting up the quanitization parameters (quantization is only for the base model)
- Setting up the Lora Config with key param such as Alpha, Dropout, r and target modules 
- Setting up the SFT Trainer using key hyperparameters and the Lora config 


# Step 1: Create datasets  
- Notebook: `dataset_prompts.ipynb` notebook 
- Generated Dataset: https://huggingface.co/datasets/abdelkader/items_prompts_full/

# Step 2: Evaluate without finetuning (base model)
- Identify the baseline performance without finetuning.  
- Notebook `base_model_evaluation.ipnyb`  


# Step 3: Funetuning with QLora 
- Notebook `finetune_qlora.ipnyb` 

# Step 4: Inference calling 
- Notebook `inference.ipnyb`








