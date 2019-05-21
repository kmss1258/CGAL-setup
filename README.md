# CGAL-setup
CGAL을 세팅해 봅시다    
환경 : VS 2015, CMake 3.9.3, Boost 1.65, CGAL 4.13.1    
Reference : http://bitly.kr/02p8xj

# CMake 다운로드
CMake를 설치. 필자는 3.9 버전 설치하였음

# CGAL setup 파일 다운로드
LINK : https://www.cgal.org/download.html    
해당 파일을 다운로드 하면 CMake를 컴파일 할 수 있는 환경이 갖춰짐

# Boost Library 다운로드
필자는 1.65.0 버전을 다운로드 하여 사용하였음.    
include 경로와 lib, bin 경로를 미리 알아두기 

```
include : E:\boost_1_65_0
lib : E:\boost_1_65_0\stage\lib
bin : E:\boost_1_65_0\stage\lib
```

# Eigen 다운로드
3.2.10 버전 다운로드    

# QT 다운로드
필자의 경우 이전에 Anaconda에서 QT 라이브러리를 다운로드 받은 적이 있어서 그걸 그대로 CMake에서 인식하였다.    
![img1](./image1.PNG)

# CGAL exe 파일 실행
CGAL을 실행하여 CMake에 필요한 파일을 압축 해제한다.

# CMake 실행

Source Code    
> C:/dev/CGAL-4.13.1    
Build    
> C:/dev/CGAL-4.13.1/build (폴더를 생성하였음)

```
EIGEN_INCLUDE_DIR : E:/eigen-eigen-b9cd8366d4e8/Eigen_3.2.10
WITH_EIGEN : check
QT 관련 : 위 사진과 같음
Boost_LIBRARY_DEBUG & RELEASE : E:/boost_1_65_0/stage/lib
Boost_INCLUDE_DIR : E:/boost_1_65_0/
```

이후, Configure, Generate, Open Project    
프로젝트가 열리면 ALL_BUILD 프로젝트를 시작 프로젝트로 지정하여, 빌드하면 된다.

# Library 연동
아래와 같이 연동하면 된다.    
    
## Include
![img2](image2.PNG)

## Library 경로 설정
![img3](image3.PNG)

## Library Files
![img4](image4.PNG)    
