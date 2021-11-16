# StyleGAN2-and-FaceMorphing

colab에서 진행하는 것을 추천 합니다.

학습 할 이미지를 넣은 후 styleGAN2-ada를 이용해 학습 합니다.

학습 이미지가 적더라도 이미지의 화질, 얼굴을 가리지 않는 이미지 등 이미지의 품질이 좋다면 좋은 결과를 얻을 수 있습니다.

아래 이미지는 styleGAN2-ada를 통해 생성된 이미지 입니다.

![chu_train28-stylegan2-kimg25000-ada-gamma1-ffhq1024](https://user-images.githubusercontent.com/40240766/141753191-ea24abb8-bfc9-414a-8594-af2b2c027df8.jpg)


# StyleGAN2

StyleGAN은 GAN에서 파생된 모델입니다.

GAN~StyleGAN2에 대한 설명을 보려면 [링크](https://www.notion.so/GAN-StyleGAN2-28db3fa1a6dd4ec5b072488beaec9072)에 가서 보시면 됩니다.

# FaceCrop

이미지를 얼굴 부분만 자르는 방법 입니다.

얼굴 이미지가 필요하시다면 다음 [링크](https://www.notion.so/a939b61381c24388a1abb85038805f64)에서 훈련 이미지를 얻으세요 !

# git lfs
git은 50MB 부터 경고가 뜨고 100MB 이상은 에러가 뜬다.

git large file storage를 설치 한다. [링크](https://git-lfs.github.com/)

설치 후 git 레포지터리 안에서 아래 코드를 입력한다.

```python
$ git lfs install
```

업로드 할 대용량 파일을 옮기고 아래 코드를 입력한다.

```python
$ git lfs track "*.zip"
$ git add .gitattributes
$ git commit -m 'message'
$ git push
```

# git lfs로 파일 다운 받기

lfs로 관리 받고 있는 파일을 다운 받으려면 아래 코드를 입력하면 된다

```python
$ git lfs pull
```

# git lfs 파일 목록 확인

```python
$ git lfs ls-files
```

# lfs가 적용된 git clone 하는 방법

lfs 까지 pull로 가져와야 사용 가능하게 복제 해 올 수 있다.

```python
$ git clone [url]
$ git lfs pull
```
