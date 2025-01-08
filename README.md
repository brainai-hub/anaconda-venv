## Intel 오픈비노 툴킷(OpenVINO Toolkits) 활용 AI 프로젝트 개발을 위한 가상 학습 환경 만들기.
  ## 아나콘다 파이썬 3.11 버전 설치
      
* 참고 사이트: https://github.com/openvinotoolkit/openvino_notebooks/wiki/Windows
( 필수 ) 
  1. 아나콘다(Anaconda) 설치
  2. 아나콘다 가상 환경 만들기
  3. 파이썬 라이브러리 및 패키지 설치
  4. 가상 환경 테스트
( 선택 )
  5. Intel OpenVINO™ Toolkit - Open Model Zoo repository 확인
  6. Visual Studio 패키지 설치

## 1. 아나콘다(Anaconda) 설치

1.1 아나콘다 파이썬 3.11 버전을 찾아 다운로드합니다.<br>
 
   - <b> 다운로드 링크:</b>  <br>
[https://repo.anaconda.com/archive/Anaconda3-2024.02-1-Windows-x86_64.exe](https://repo.anaconda.com/archive/Anaconda3-2024.02-1-Windows-x86_64.exe) <br><br>
   - <b> 아나콘다 Archive 링크:</b>  <br>   
 <a href="https://repo.anaconda.com/archive/" target="_blank"> https://repo.anaconda.com/archive/ </a>


  
1.2 다운 받은 파일을 찾아 설치합니다. 설치 시 주의할 내용은 아래 이미지를 참고하세요.
 
  <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-01.PNG" style="width:501px;height:390px;">

## 2. 아나콘다 가상 환경 만들기

 #### 2-1. 시작 메뉴에서 Anaconda3 (64-bit)폴더를 찾습니다. Anaconda Prompt (Anaconda3) 메뉴를 오른쪽 마우스 버튼을 클릭한 후 [자세히]-[관리자 권한으로 실행]을 찾아 왼쪽 마우스 버튼을 클릭하여 실행합니다.  

 <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-02.PNG">
 
 #### 2-2. 다음 순서대로 명령을 실행하여 가상 환경을 만듭니다.
 - (base) C:\WINDOWS\system32>cd\
 - (base) C:\mkdir BrainAI
 - (base) C:\cd BrainAI
 - (base) C:\BrainAI>conda create --name BrainAI python==3.11.8 anaconda
 - (base) C:\BrainAI>conda activate BrainAI
 - (BrainAI) C:\BrainAI>

## 3. 인텔 OpenVINO notebooks 다운 받아 C:\BrainAI\폴더에 위치시키기
  인텔 OpenVINO notebooks 다운로드 링크입니다. <br>
  https://github.com/openvinotoolkit/openvino_notebooks.git
  - (BrainAI) C:\BrainAI>cd openvino_notebooks
    
## 4. 파이썬 라이브러리 및 패키지 설치

  학습에 필요한 라이브러리 및 패키지를 설치합니다. pip 최신 버전, opencv-python, openvino 등
 - (BrainAI) C:\BrainAI>openvino_notebooks>pip install --upgrade --user pip
 - (BrainAI) C:\BrainAI>openvino_notebooks>pip install --upgrade pip wheel setuptools
 - (BrainAI) C:\BrainAI>openvino_notebooks>pip install -r requirements.txt
 - (BrainAI) C:\BrainAI>openvino_notebooks>pip install openvino>=2024.0.0
 - (BrainAI) C:\BrainAI>openvino_notebooks>pip install opencv-python
 - (BrainAI) C:\BrainAI>openvino_notebooks>pip install ipywidgets==8.1.2
 - (BrainAI) C:\BrainAI>openvino_notebooks>jupyter lab

## 4. 가상 환경 테스트
 - 주피터 랩에서 아래 코드 입력 <br>
  <img src="https://github.com/brainai-hub/anaconda-venv/blob/main/Anaconda-03.png" >
* OpenVINo 버전이 출력되면 가상 환경이 정상적으로 설치된 것입니다.\

##### 주피터 랩이 크롬 브라우저에서 자동 실행이 안될 경우 아래 링크를 참고하세요.
* 참고 링크: [http://egloos.zum.com/doodoodoo/v/2244082](https://zephyrus1111.tistory.com/336)
  <img src="https://github.com/brainai-hub/anaconda-venv/blob/main/Anaconda-04.PNG" >


## 5. Visual Studio 패키지 설치

 - <b> 다운로드 링크: </b> https://aka.ms/vs/17/release/vc_redist.x64.exe
 * 참고 링크 : https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170 <br>
  <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-venv-04.JPG" style="width:760px;height:400px;">
  * 설치 후 컴퓨터를 재시작합니다.

## 참고. Intel OpenVINO™ Toolkit - Open Model Zoo repository 확인
  
  인텔 OpenVINO Pre-trained 모델 파일 다운로드 하고 싶으면 아래 링크를 참고하세요.<br>
  [(https://storage.openvinotoolkit.org/repositories/open_model_zoo/2023.0/models_bin/1/)](https://storage.openvinotoolkit.org/repositories/open_model_zoo/2023.0/models_bin/1/)

  인텔 OpenVINO Pre-trained 모델에 대해 자세히 알아보고 싶으면 아래 링크를 참고하세요. <br>
  [(https://docs.openvino.ai/2023.3/get_started.html)](https://docs.openvino.ai/2023.3/home.html) <br>
  
  인텔 OpenVINO Model Zoo 다양한 Pre-trained 모델을 확인할 수 있습니다. <br>
  https://github.com/openvinotoolkit/open_model_zoo/tree/master/models 


#### Tip. 가상 환경 삭제하기

  가상 환경을 완전히 삭제하고 다시 설치하고 싶으면 다음을 참고하세요. <br>
 - Anaconda Prompt(Anaconda3) 창 열기
 - (Base) C:\WINDOWS\System32\conda info --envs
    * 가상환경이름 확인
 - (Base) C:\WINDOWS\System32\conda env remove --n 가상환경이름 

수고 하셨습니다. <br>
이제 AI Project 개발을 위한 환경이 모두 갖추어졌습니다.

