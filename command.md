python eval.py \
--trained_model=weights/yolact_base_54_800000.pth \
--score_threshold=0.15 \
--top_k=15 \
--video_multiframe=1 \
--video=/home/yuya/src_dir/tennis_technology/input/tennis_game/movie/Kei/match_01.mp4

--trained_model=weights/yolact_plus_resnet50_54_800000.pth \

pip install https://download.pytorch.org/whl/cu100/torch-1.1.0-cp36-cp36m-linux_x86_64.whl
pip install https://download.pytorch.org/whl/cu100/torchvision-0.3.0-cp36-cp36m-linux_x86_64.whl

# PTX JIT compilation failed
RuntimeError: /pytorch/torch/csrc/jit/fuser/cuda/fused_kernel.cpp:137: a PTX JIT compilation failed
https://github.com/pytorch/pytorch/issues/21004

## solution 
pip3 install https://download.pytorch.org/whl/cu100/torch-1.1.0-cp36-cp36m-linux_x86_64.whl
pip3 install https://download.pytorch.org/whl/cu100/torchvision-0.3.0-cp36-cp36m-linux_x86_64.whl
