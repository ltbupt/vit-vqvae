## vit-vqvae test_vit_patch4_01
第一次尝试使用vit结构，在sketch数据集上，有像素块问题
## 第一次debug test_vit_debug_01
使用cifar10数据集，发现在普通的image上未出现像素块问题
## 第二次debug test_vit_debug_02
使用sketch数据集，将reconstruction loss * 10，保证三个loss间数量级一致，结果仍存在之前的像素块问题，但相比于初次这一问题有所缓解
## final weight
/root/sketch_mask/beit_lt/codebook_weight/vit_vae_16_224_8192.pt
- original
![original](https://user-images.githubusercontent.com/89373310/195238018-2140bf03-d530-4a74-880f-2393fb0fcb04.jpg)
- reconstruction
![reconstruction](https://user-images.githubusercontent.com/89373310/195238095-849aad8f-5328-4b06-8fd6-9a76daf6d150.jpg)

