# URA-LLaMa

## Overview

## Running pipeline
### Run on local computer
```bash
vieval --mode generation \
               --model_name ura-hcmut/MixSUra \
               --dataset_name zalo_e2eqa \
               --prompting_strategy 0 \
               --fewshot_prompting True \
               --seed 42
```
### Run on TGI
```bash
vieval --mode generation \
               --model_name ura-hcmut/MixSUra \
               --dataset_name zalo_e2eqa \
               --prompting_strategy 0 \
               --fewshot_prompting True \
               --seed 42 \
               --tgi http://127.0.0.1:10025
```
### Run on GPT (gpt-3.5-turbo, gpt-4)
```bash
vieval --mode generation \
               --model_name gpt-4 \
               --dataset_name zalo_e2eqa \
               --prompting_strategy 0 \
               --fewshot_prompting True \
               --seed 42
```
## Evaluation
```bash
vieval --mode evaluation \
               --model_name gpt-4 \
               --dataset_name zalo_e2eqa \
               --prompting_strategy 0 \
               --fewshot_prompting True \
               --seed 42 \
               --output_dir results \
               --out_eval_dir out_new
```

## End2End Pipeline
```bash
vieval --mode end2end \
               --model_name gpt-4 \
               --dataset_name zalo_e2eqa \
               --prompting_strategy 0 \
               --fewshot_prompting True \
               --seed 42 \
               --output_dir results \
               --out_eval_dir out_new
```
## License and Usage Agreement

## Citation
