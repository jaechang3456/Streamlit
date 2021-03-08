### 1. Conda 이용한 파이썬 가상환경 설정방법
우선 다음 링크에서 아나콘다를 설치해 줍니다. 
https://www.anaconda.com/products/individual 
conda create -n streamlit 코드를 입력하여, 가상환경 상황을 만들어줍니다.
activate streamlit 을 입력하여
C:\Users\5-24\Documents\Streamlit\day02>C:/Users/5-24/anaconda3/Scripts/activate

(base) C:\Users\5-24\Documents\Streamlit\day02>conda activate streamlit

(streamlit) C:\Users\5-24\Documents\Streamlit
다음과 같이 나오면, 성공적으로 가상환경을 실행 한 것입니다.

다음으로 deactivate 코드를 이용하여 가상환경을 해제 할 수 있습니다.
conda env export > steamlit.yaml 를 입력하여, 가상환경을 yaml 파일로 내보낼 수 있고
conda env create -f streamlit.yaml 를 이용하여 가상환경 파일을 불러와 사용 할 수도 있으며,
conda env remove -n my_python_env 를 이용하여 가상환경을 제거 할 수도 있습니다.

### 2. Streamlit 머신러닝 대시보드 개발 환경 설정 with Visual Studio Code
![image](https://user-images.githubusercontent.com/78472987/110298634-27409580-8038-11eb-909b-582371b9604f.png)
먼저 왼쪽 메뉴 중 가장 위에 있는 문서모양 버튼을 클릭하여 줍니다.
그럼 Open Folder 라고 파란 버튼이 나오게 됩니다.
버튼을 클릭해서 미리 가상환경까지 만들어 두었던 streamlit을 선택해 줍니다

그럼 Open Folder 라고 파란 버튼이 나오게 됩니다.

streamlit 폴더를 선택 한 후 OK를 눌러줍니다.
streamlit폴더의 내용이 보여지지만, 아직 아무 파일을 만들지 않아서 설정해두었던 가상환경 폴더만 보여집니다.
![image](https://user-images.githubusercontent.com/78472987/110298925-75ee2f80-8038-11eb-9efb-b11052789e78.png)

맨 왼쪽 메뉴 중에 가장 아레에 있는 메뉴를 누르고, 검색창에 Python 검색 후 Python을 설치 해 줍니다.

![image](https://user-images.githubusercontent.com/78472987/110299047-9ae2a280-8038-11eb-8932-eaa5d30267c7.png)

new file 버튼을 눌러, 새로운 파일을 생성해 준 후 이름을 name.py로 하면, VSCode에서 Python파일로 인식합니다.


출처: https://somjang.tistory.com/entry/PythonVisual-Studio-Code-개발환경-설정하기feat-Ubuntu [솜씨좋은장씨]


### 3. Streamlit 동작시키기 위한 기본 코드와, 실행 명령어
먼저 Streamlit을 설치합니다.
python --version 3.6이상이어야 설치 가능합니다.
pip install streamlit 입력
Ctrl + Shift + P 입력하여 Python : Selct Interpreter 선택하여 streamlit:conda 선택합니다.
New Terminal을 생성해주고 아래와 같이 나오면 동작 시작입니다.

![image](https://user-images.githubusercontent.com/78472987/110298037-74703780-8037-11eb-9d49-3b52a5baf2b5.png)
![image](https://user-images.githubusercontent.com/78472987/110297953-560a3c00-8037-11eb-9695-bf4a683bc425.png)

Streamlit이 동작하기 시작했다면, Streamlit환경에서 실행할 app을 만들고, 새로 만든 Terminal에
streamlit run 파일이름.py 입력하면 실행됩니다.
