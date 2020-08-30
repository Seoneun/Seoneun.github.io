---
title: "Anaconda Virtual Environment"
date: 2020-08-30 23:08:28 -0400
categories: Anaconda
---
**아나콘다 가상환경(Anaconda Virtual Environment)**

아나콘다는 사용자가 개발할 수 있는 복수의 환경을 독립적으로 만드는 것이 가능합니다.   
가상환경을 만듦으로서 base를 오염시키지 않을 수 있고 혹여나 패키지 간의 문제가 발생할 경우 문제를 해결하기 보다는 단순히 그 환경을 지우고 새로운 환경을 만들시면 됩니다.   

**아나콘다 가상환경 만들기(window기준)**

1. Anaconda Navigator를 실행합니다.   
2. CMD.exe Prompt를 Launch합니다. 만약 프롬프트가 설치되어 있지 않다면 install하시고 Launch하시면 됩니다.   
3. 프롬프트에 'conda create -n my_python_env'를 입력하시면 됩니다. 여기서 'my_python_env'는 만들고자 하는 가상환경의 이름입니다. 원하시는 대로 이름을 바꿔 사용하시면 됩니다.   

**가상환경에 python설치하기**

가상환경에 python을 설치하기 위해서는 'conda create -n my_python_env python=_version_'을 누르시면 됩니다. 여기서 '_version_' 부분에 원하시는 파이썬 버전을 입력하시면 됩니다.   
ex) python 3.4버전 설치 'conda create -n my_python_env python=3.4'
