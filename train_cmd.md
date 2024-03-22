
1.新建一次训练
python scripts/train.py --task=bipedv5_ppo --run_name newrun --headless --num_envs 4096
2.继续训练
python scripts/train.py --task=bipedv5_ppo  --resume --load_run Mar14_15-43-51_  --num_envs 4096 --headless
//可视化查看训练情况
python scripts/train.py --task=bipedv5_ppo  --resume --load_run Mar14_15-43-51_  --num_envs 256
3.推理
python scripts/play.py --task=bipedv5_ppo --run_name test314 --checkpoint 1500  --num_envs 20 //加载model_1500.pt
python scripts/play.py --task=bipedv5_ppo --run_name one_pri   --num_envs 20

