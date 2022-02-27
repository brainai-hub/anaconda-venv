# 인공지능을 배우기 위한 가상 학습 환경 만들기
  
  <a href="https://www.intel.com/content/www/us/en/corporate/artificial-intelligence/digital-readiness-home.html" target="_blank"> Intel® Digital Readiness Programs </a> <br>
  
  AI for Youth <br>
  For high school students.

  Module 5, Module 6, Module 8, Module 9

  - Anaconda python 3.8
  - Tensorflow 2.8
  <br><br>

## 1. 아나콘다(Anaconda) 설치
 
 다운로드 링크: https://repo.anaconda.com/archive/Anaconda3-2021.05-Windows-x86_64.exe <br>
 <a href="https://repo.anaconda.com/archive/" target="_blank"> <img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda-venv-02.JPG" style="width:500px;height:600px;"> </a>
 
## 2. Visual Studion 패키지 설치
 참고 사이트 : https://docs.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170 <br>
 다운로드 링크: https://aka.ms/vs/17/release/vc_redist.x64.exe

## 3. 가상 학습 환경 만들기
 - (base) C:\WINDOWS\system32\cd\
 - (base) C:\mkdir BrainAI
 - (base) C:\cd BrainAI
 - (base) C:\BrainAI>conda update -n base -c default conda
 - (base) C:\BrainAI>conda create --name BrainAI python=3.8 anaconda
 - (base) C:\BrainAI>conda activate BrainAI
 - (BrainAI) C:\BrainAI>

## Tensorflow 2.8 설치하기
 - (BrainAI) C:\BrainAI>pip install --upgrade --user pip
 - (BrainAI) C:\BrainAI>pip install --upgrade tensorflow
 - (BrainAI) C:\BrainAI>pip install --opencv-python
 - (BrainAI) C:\BrainAI>pip install imultils
 - (BrainAI) C:\BrainAI>pip install pyserial
 - (BrainAI) C:\BrainAI>jupyter lab

## 가상 학습 환경 테스트
<img src="https://github.com/BrainAI-Lab/venv/blob/main/Anaconda3-2021.05-Windows-x86_64-07.JPG">
