운영체제프로젝트 readme파일
=====================
# 실행환경
vscode내부에서 컴파일해서 실행하였다.

# 구현내용, 방법
named pipe를 mkfifo()를 사용해 Server에서 FIF01, FIF02 순서대로 2개를 만들었다.

요구사항에 적힌 내용대로 Client와 Server에서 open하였다.

사용자들이 정의된 대로 입력하면 클라이언트에서 입력을 받아들인다. 

Client에서 정의된 named pipe를 통해 파일 access요청하면 server에서 fork()를 사용해 child 를 만들어서 응답하게 하였다.

while(1)을 사용해 반복하여 수행하게 하였다. 

exit()을 사용해 임무완수한 child는 종료되게 하였다.

switch()를 사용해 w인 상황과 r인 상황을 가정해 수행하도록 하였다.

client가 write()를 사용해 Server에 정보를 전달하면 Server는 read()를 이용하여 내용을 저장한다.

client가 read()를 사용해 정보를 가져오려하면 Server는 write()를 이용해 Client에게 정보를 전달한다.



<!--
**imminsoo/imminsoo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
