model_mnist, model_fmnist는 pretrained classifier model
model_LSGAN_g_3 은 pretrained LSGAN generator
VAE_FMNIST_32, VAE_MNIST_10은 laten vector 크기가 각각 32, 10인 pretrained VAE

이 파일들이 기본경로로만 잡혀있다면,
이미지와, TSNE 이미지 생성
mnist의 경우 첫번째가 ga를 이용한 사진, 두번째가 원래 이미지, 세번째가 원래이미지를 오토인코더로 재구현한 사진
fmnist의 경우 첫번째가 ga를 이용한 사진, 두번째가 generator가 만들어낸 사진
