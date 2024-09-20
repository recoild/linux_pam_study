### PAM

인증 과정을 설정 파일로 관리할 수 있게 해주는 모듈

인증 설정 파일들 경로: /etc/pam.d

명령어들(passwd, su…)에 대해 설정 파일들이 있습니다.

![image](https://github.com/user-attachments/assets/cadbfa7c-b2a0-494c-b6f9-e9c09009392a)

minlen=1을 걸어서 passwd할 때 패스워드 길이를 1로 제한할 수 있습니다.

## 패스워드 시도 횟수 초과

![image](https://github.com/user-attachments/assets/0db207bc-7eb3-4b52-9423-a9c545b0892f)

만약, adduser 명령어로 유저 생성 시 패스워드 설정 횟수 초과(3회 초과)를 하게 되면 자동으로 패스워드 입력을 무시합니다.<br/>
그러나, 이는 패스워드 입력 우회한 것이 아니라 패스워드 미입력 상태로 유저가 생성된 것이므로 추후 해당 유저로 로그인 후 인증 시도를 하게되면 패스워드 입력이 안됩니다.
