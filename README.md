## Intel® AI for Youth 프로그램 학습을 위한 가상 학습 환경 만들기.
  ## 아나콘다 파이썬 3.8 버전 설치
      
<a href="https://www.intel.com/content/www/us/en/corporate/artificial-intelligence/digital-readiness-home.html" target=_blank> Intel® Digital Readiness Programs </a>  중 AI for Youth Program의 <br>
  Stage 3. 실력키우기 / Module 5, Module 6, Module 8, Module 9, Module 10 <br>
  Stage 4. 소셜임팩트 창출하기 / Module 11 Use Cases 실습을 위한 가상 학습 환경 만들기에 대한 도움 자료입니다. <br>
  AI for Youth 참고 사이트: https://brainai.kr/ai4y/ <br>
  AI for Youth 프로그램 코딩 실습 및 프로젝트 개발 실습은 초보자도 쉽게 시작할 수 있는 아나콘다 주피터 랩 환경을 이용합니다.<br>
  AI for Youth 프로그램을 이용한 AI 학습을 위해 다음 순서로 가상 학습 환경을 만들어 봅시다.
  
  1. 아나콘다(Anaconda) 설치
  2. Visual Studio 패키지 설치
  3. 아나콘다 가상 학습 환경 만들기
  4. 라이브러리 및 패키지 설치

## 1. 아나콘다(Anaconda) 설치

1.1 아나콘다 파이썬 3.8 버전을 아나콘다 Archive 폴더에서 찾아 다운로드합니다.<br>
 
   - <b> 다운로드 링크:</b> https://repo.anaconda.com/archive/Anaconda3-2021.05-Windows-x86_64.exe <br>
 <a href="https://repo.anaconda.com/archive/" target="_blank"> 
  
   - 참고 링크: https://repo.anaconda.com/archive/<br>
   - 참고 링크: https://docs.anaconda.com/anaconda/packages/py3.8_win-64/ <br>
   <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-venv-02.JPG" style="width:669px;height:257px;"> </a>

1.2 다운 받은 파일을 찾아 설치합니다. 설치 시 주의할 내용은 아래 이미지를 참고하세요.
 
  <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-venv-03.JPG" style="width:849px;height:335px;">

  * 참고 링크: 아나콘다 파이썬 3.8 버전 설치 링크 : https://docs.anaconda.com/anaconda/install/windows/
 
## 2. Visual Studio 패키지 설치

  - <b> 다운로드 링크: </b> https://aka.ms/vs/17/release/vc_redist.x64.exe

  - 참고 링크 : https://docs.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170 <br>

  <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-venv-04.JPG" style="width:760px;height:200px;">

## 3. 아나콘다 가상 학습 환경 만들기

  Anaconda Promt (Anaconda3) Command 창(아래 이미지 참고)에서 다음 순서대로 명령을 실행하여 가상 학습 환경을 만듭니다.
 
 <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-venv-05.JPG" style="width:369px;height:156px;">
 
 - (base) C:\WINDOWS\system32>cd\
 - (base) C:\mkdir BrainAI
 - (base) C:\cd BrainAI
 - (base) C:\BrainAI>conda create --name BrainAI python=3.8 anaconda
 - (base) C:\BrainAI>conda activate BrainAI
 - (BrainAI) C:\BrainAI>

## 4. 라이브러리 및 패키지 설치

  학습에 필요한 라이브러리 및 패키지를 설치합니다. pip 최신 버전, 텐서플로우, 넘파이, opencv-python, Pyserial, imutils, openvino, openvino-dev(버전 2022.1.0) 등
  <br><br>
 
 - (BrainAI) C:\BrainAI>pip install --upgrade --user pip
 - (BrainAI) C:\BrainAI>pip install tensorflow==2.5
 - (BrainAI) C:\BrainAI> pip install numpy==1.19.5
 - (BrainAI) C:\BrainAI>pip install opencv-python
 - (BrainAI) C:\BrainAI>pip install imutils
 - (BrainAI) C:\BrainAI>pip install pyserial
 - (BrainAI) C:\BrainAI>pip install openvino==2022.1.0
 - (BrainAI) C:\BrainAI>pip install openvino-dev==2022.1.0
 - (BrainAI) C:\BrainAI>pip install openvino-dev[tensorflow]
 - (BrainAI) C:\BrainAI>jupyter lab

## 5. 가상 학습 환경 테스트

 - 주피터 랩에서 아래 코드 입력 <br>
  <img src="https://github.com/BrainAI-Lab/venv/blob/main/tensor_version_p.JPG" >
  
<b> Tensorflow 2.#.# 버전이 출력되면 가상 학습 환경이 정상적으로 설치된 것입니다. </b>


## Tip. 가상 학습 환경 삭제하기

  가상 학습 환경을 완전히 삭제하고 다시 설치하고 싶으면 아래 링크를 참고하세요. 
    * Anaconda Prompt(Anaconda3)에서 
 - (Base) C:\WINDOWS\System32\conda info --envs
    * 가상환경 이름 확인
 - (Base) C:\WINDOWS\System32\conda env remove --n 가상환경이름 

## Tip. OpenVINO™ Toolkit - Open Model Zoo repository
 - Git 다운 로드 링크
https://github.com/git-for-windows/git/releases/download/v2.35.1.windows.2/Git-2.35.1.2-64-bit.exe
 - (BrainAI) C:\BrainAI>git clone --depth=1 https://github.com/openvinotoolkit/openvino_notebooks.git


  인텔 OpenVINO Pre-trained 모델에 대해 자세히 알아보고 싶으면 아래 링크를 참고하세요. 

  참고 링크: https://docs.openvino.ai/2022.1/index.html

  인텔 OpenVINO Pre-trained 모델 파일 다운로드 하고 싶으면 아래 링크를 참고하세요.
  
  참고 링크: https://storage.openvinotoolkit.org/repositories/open_model_zoo/2022.1/models_bin/
  
### 주피터랩 크롬 브라우저에 자동 실행이 안될 경우 아래 링크를 참고하세요.
  참고 링크: http://egloos.zum.com/doodoodoo/v/2244082
  
### 수고하셨습니다. 

