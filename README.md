### 강태욱박사님 강좌
```
fastcampus_yolo/
│
├── README.md
│
└── examples/
    └── filter.ipynb
```
##### 엣지 검출 (Edge Detection)
엣지 검출은 이미지에서 경계선이나 윤곽선을 찾아내는 작업입니다. 엣지 검출 필터는 픽셀 값이 급격히 변하는 부분을 강조하여 이미지의 경계선 부분을 더 잘 보이게 해주며,  필터(커널)를 통해 엣지 검출, 샤프닝, 블러링 등의 효과를 이미지에 적용하여 그 특징을 강조하거나 변환할 수 있다는 의미
예제 커널
Sobel 커널 (수직 엣지 검출)
``` bash
sobel_vertical = np.array([[1, 0, -1],
                           [2, 0, -2],
                           [1, 0, -1]])
```
``` bash
Sobel 커널 (수평 엣지 검출)
sobel_horizontal = np.array([[1, 2, 1],
                             [0, 0, 0],
                             [-1, -2, -1]])
```
Laplacian 커널 (엣지 검출)
```
laplacian = np.array([[0, 1, 0],
                      [1, -4, 1],
                      [0, 1, 0]])
```
샤프닝 (Sharpening)
샤프닝은 이미지의 세부사항을 더 선명하게 하는 작업입니다. 이를 통해 이미지의 윤곽선과 디테일을 강조할 수 있습니다.

예제 커널
샤프닝 커널 1
```
sharpen1 = np.array([[0, -1, 0],
                     [-1, 5, -1],
                     [0, -1, 0]])
```
샤프닝 커널 2
```
sharpen2 = np.array([[-1, -1, -1],
                     [-1, 9, -1],
                     [-1, -1, -1]])
```


