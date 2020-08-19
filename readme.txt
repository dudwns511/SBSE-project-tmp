model_mnist, model_fmnist는 pretrained classifier model
model_LSGAN_g_3 은 pretrained LSGAN generator
VAE_FMNIST_32, VAE_MNIST_10은 laten vector 크기가 각각 32, 10인 pretrained VAE

이 파일들이 기본경로로만 잡혀있다면,
sbse_project_final.py 파일을 실행하여
이미지와, TSNE 이미지 생성
mnist의 경우 첫번째가 ga를 이용한 사진, 두번째가 원래 이미지, 세번째가 원래이미지를 오토인코더로 재구현한 사진
fmnist의 경우 첫번째가 ga를 이용한 사진, 두번째가 generator가 만들어낸 사진

TSNE이미지의 경우 classifier의 output 전 layer의 feature값을 사용하여 시각화
gen_...png 는 ga를 이용하여 만들어낸 이미지를 origin이미지와 비교하여 색을 입혀서 표현
origin_...png는 트레이닝 셋에서 무작위로 뽑아온(mnist의 경우 5000개, fmnist의 경우 10000개) 이미지들의 위치를 표현
