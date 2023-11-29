# Redis

 컴파일<br/>
 ~/redis-7.2.2/src 위치에서 아래의 명령어를 통해 코드를 모듈로 컴파일<br/>
 gcc -fPIC pangmodule.c -shared -o pangmodule.so <br/>
<br/>
<br/>
 모듈로드<br/> 
 ~/redis-7.2.2 위치에서 아래의 명령어를 통해 모듈을 서버에 로드 (업로드한 파일에 pangmodule.so가 미리 준비되어 있습니다.)<br/>
 redis-server –loadmodule ./pangmodule.so
<br/>
<br/>
redis-cli에서 pang 명령 시 PUNG 반환
