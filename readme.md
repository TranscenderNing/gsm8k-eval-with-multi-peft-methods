nohup python train.py --peft_method lora > train_lora.log 2>&1 &
nohup python train.py --peft_method dora > train_dora.log 2>&1 &
nohup python train.py --peft_method rslora > train_rslora.log 2>&1 &
nohup python train.py --peft_method adalora > train_adalora.log 2>&1 &
nohup python train.py --peft_method pissa > train_pissa.log 2>&1 &
CUDA_VISIBLE_DEVICES=5 nohup python train.py --peft_method milora > train_milora_min_max.log 2>&1 &

# infer 
predict()


