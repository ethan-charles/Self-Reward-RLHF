## Self Rewarding Language Model

Implement for [Self-Rewarding Language Model paper](https://arxiv.org/abs/2401.10020) from MetaAI.

Our paper is Here! [Exploring Self-Learning and Teacher-Guided
Paradigms in Language Model Alignment](https://github.com/ethan-charles/Self-Reward-RLHF/blob/main/Exploring_Self-Learning_and_Teacher-Guided_Paradigms_in_Language_Model_Alignment.pdf)

[](https://github.com/ethan-charles/Self-Reward-RLHF/blob/main/EECS%20598%20Poster_v2.png)

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




