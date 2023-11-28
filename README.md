# Redis

# 컴파일
# ~/redis-7.2.2/src 위치에서 아래의 명령어를 통해 코드를 모듈로 컴파일
# gcc -fPIC pangmodule.c -shared -o pangmodule.so 


# 모듈로드 
# ~/redis-7.2.2 위치에서 아래의 명령어를 통해 모듈을 서버에 로드 (업로드한 파일에 pangmodule.so가 미리 준비되어 있습니다.)
# redis-server –loadmodule ./pangmodule.so

# redis-cli에서 pang입력시 PUNG 반환
