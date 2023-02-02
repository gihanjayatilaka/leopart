<!-- srun --pty --account=abhinav --qos=high --time=8:00:00 --gpus-per-node=1 --mem-per-cpu=64000 bash
srun --pty --account=abhinav --qos=high --time=8:00:00 --gres=gpu:1 --ntasks 4 --mem=64gb bash -->
srun --pty --account=abhinav --qos=high --time=8:00:00 --gres=gpu:rtxa6000:2 --ntasks 8 --mem=128gb bash
<!-- 1080ti:1
gpu:rtxa6000:1 -->

cd leopart
export PYTHONPATH=$(pwd)