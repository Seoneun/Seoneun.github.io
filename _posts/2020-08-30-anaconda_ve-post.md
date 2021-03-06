---
title: "Anaconda Virtual Environment"
date: 2020-08-30 23:08:28 -0400
categories: Anaconda
comments: true
---
**아나콘다 가상환경(Anaconda Virtual Environment)**

아나콘다는 사용자가 개발할 수 있는 복수의 환경을 독립적으로 만드는 것이 가능합니다.   
가상환경을 만듦으로서 base를 오염시키지 않을 수 있고 혹여나 패키지 간의 문제가 발생할 경우 문제를 해결하기 보다는 단순히 그 환경을 지우고 새로운 환경을 만들시면 됩니다.   

**아나콘다 가상환경 만들기(window기준)**

1. Anaconda Navigator를 실행합니다.   
2. CMD.exe Prompt를 Launch합니다. 만약 프롬프트가 설치되어 있지 않다면 install하시고 Launch하시면 됩니다.   
3. 프롬프트에 `conda create -n my_python_env`를 입력하시면 됩니다. 여기서 'my_python_env'는 만들고자 하는 가상환경의 이름입니다. 원하시는 대로 이름을 바꿔 사용하시면 됩니다.   

**가상환경에 python설치하기**

가상환경에 python을 설치하기 위해서는 `conda create -n my_python_env python=_version_`을 누르시면 됩니다. 여기서 `_version_` 부분에 원하시는 파이썬 버전을 입력하시면 됩니다.   
ex) python 3.4버전 설치 `conda create -n my_python_env python=3.4`

**가상환경 실행**

macOS/Linux   
`source activate my_python_env`

Windows   
`activate my_python_env`

를 프롬프트에 입력하시면 됩니다. 프롬프트에서 (base)부분이 (my_python_env)으로 바뀌었다면 제대로 동작하는 것입니다.   
추가로 Anaconda Navigator에서 Applications on 옆에 리스트를 통해 원하는 가상환경을 실행시킬 수 있습니다.

**가상환경 종료**

macOS/Linux   
`source deactivate`

Windows   
`deactivate`

를 프롬프트에 입력하시면 됩니다.

**가상환경 리스트 출력**

`conda env list`를 프롬프트에 입력하면 설치된 가상환경 목록 전체를 확인할 수 있습니다.

**가상환경 제거**

`conda env remove -n my_python_env`를 입력하여 my_python_env 가상환경을 제거할 수 있습니다.
