## Self Rewarding Language Model

Implement for [Self-Rewarding Language Model paper](https://arxiv.org/abs/2401.10020) from MetaAI.

### Advanced method for small language model:

 - Teacher reward llm
 - Teacher instruct llm

## Installation
```
pip install -r requirements.txt
```


#### step 1: SFT (M0 -> M1)
```
python srlm/SFT.py
```
#### step 2: Generates dpo dataset 
```
python srlm/Generate.py
```
#### step 3: DPO (M1 -> M2)
```
python srlm/DPO.py
```

## Usage

self reward llm
```
python run_self_reward.py <--dataset> <--model> <--output> <--user>
```
Teacher reward llm
```
python run_teacher_reward.py <--dataset> <--model> <--output> <--user>
```
Teacher instruct llm
```
python run_teacher_instruct.py <--dataset> <--model> <--output> <--user>
```




