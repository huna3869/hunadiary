한양대학교 ERICA 프로그래밍 경진대회 개최까지
============
2016.05.19 한양대학교 ERICA 게스트하우스에서 작성<br>
2016.05.24 한양대학교 ERICA 캠퍼스에서 업로드
<br>
<br>
드디어 3시간에 걸친 대회가 끝났습니다. 큰 짐을 하나 덜어 낸 것 같이 느껴집니다.<br>
지난 3주는 정말 바쁜 기간이었습니다. 한양대학교 ERICA 프로그래밍 경진대회, HEPC의 개최준비를 했어야 했기 때문입니다. 저는 대회 접수 개시 3일 전 쯤, 대회 홈페이지를 만들어 달라는 이야기를 듣게 됩니다. 3일은 좀 빡빡한 일정이었습니다만, 그럭저럭 반응성도 작동하며, 접수도 되는 그럴싸해 보이는 [홈페이지](http://hepc.hycse.net)의 제작을 할 수 있었습니다. 대회 홈페이지는 자주 쓰일 그런 홈페이지가 아니기 때문에, 솔직히 대충 엔진에 테마를 덧씌운, 그런 식의 홈페이지를 만들 생각이었습니다만, 워낙 주변 지인분들이 이러한 일을 할 때 쓴 소리를 신나게 했던 저인지라, 대충 만들거나 하면 일이 터질까 두려워 자체 제작을 했습니다. 대회 접수 중 다행히 큰 문제는 일어나지 않았지만, 제가 실수로 문자열 검사를 위한 정규식을 잘못 작성하였고, 대회 초기에는 -,_가 들어간 이메일은 접수가 되지 않는 해프닝이 일어나기도 했습니다. 또한, 팀명에 대한 문자열 검사가 제대로 이루어지지 않았다는 사실을 깨달은 건 대회 접수 시작 일주일 뒤였습니다. 다행히 아무도 부정 입력을 넣어주지 않아서 문제없이 접수가 이루어졌습니다. <br><br>
홈페이지의 준비가 끝나고, 대회 문제의 출제와 채점 서버의 준비를 해야 했습니다. 대회 문제는 저를 포함한 학부생 출제진 5명이 구성되었습니다. 각 3문제씩을 뽑아 15문제 중, 10문제를 뽑아 최종 문제를 내기로 했습니다. 저도 원래 3문제를 출제를 했습니만, 대회에 출제하기에는 문제의 난이도가 조금 높다는 의견이 많아 출제하지 않고, 채점서버의 제작에 몰두했습니다. 채점 서버는 처음에는 대회 홈페이지가 있는 교수님의 서버를 이용하려고 했습니다. (한양대학교 내에 물리적 서버를 두지 못한 이유는, 정보실에 승인을 받아 포트와 IP를 열기에는 자원과 시간이 너무 부족했기 때문입니다.) 하지만 필요한 프로그램들(스코어보드를 위해서는 Node가 필요했습니다.)의 설치에 필요한 권한을 얻지 못하는 문제로 인해서, 어쩔 수 없이 AWS를 쓰게 되었습니다. AWS에 채점 서버를 올리고, 또 다른 인스턴스에는 결과를 보여줄 스코어보드를 올렸습니다. 스코어보드 프로그램을 올리는 데에도 문제가 몇가지 있었는데, 스코어보드는 최신 버전의 PC^2와 호환이 되지 않았기 때문에, 구 버전으로 서버를 다시 세팅해야 했습니다. 서버들이 제대로 작동하지 않아 고생을 엄청 했고, (후에 서버 성능이 낮아 메모리 부족으로 프로그램이 오작동을 일으켜왔던 것으로 밝혀졌습니다.) 그래서 스트레스 테스트도 제대로 못한 채로 대회 당일에 돌입을 했습니다.<br><br>
대회 당일에도 문제는 많았습니다. 일단, 교수님이 주신 AP 장치는 제대로 동작 하지 않았습니다. 결국 게스트하우스의 네트워크를 쓰도록 유도했습니다. 가장 큰 문제는 대회 개최 1시간 전에 일어났습니다. 대회 서버가 채점 시스템의 연결조차 견디지 못하고 뻗어버리는 것입니다. AWS를 이용한게 그나마 다행이었습니다. 작년 창업캠프 때 700$를 물게 된 팀들을 보아 왔기 때문에 조금 불안하기는 했지만, 지금 와서는 선택지가 없었기에, 성능을 높게 올리고 최종 테스트를 했습니다. 대회 직전까지 작동을 잘 하지 않던 스코어보드가 대회 시작 직전에 작동하기 시작한 것은 굉장한 요행이었습니다.<br><br>
대회 중간에 문제들에 대한 질문들이 쏟아지거나(대부분은 출제 미숙이었습니다.), 채점 프로그램이 출력 스트림이 넘쳐서 잠시 꺼지는 일이 있긴 했지만, 대회는 거의 성공적으로 끝났습니다. 대회 마지막에 스코어보드를 시상식모드로 돌리는 방법을 잘 몰라서 시간을 잡아먹은게 대회에서 저지른 마지막 실수일거라 생각했습니다.<br><br>
대회 종료 후, 서버를 다 끄고 돌아서고 나서, 문제에 이상이 있다고 하며 Rejudge를 요청한 팀이 있었습니다. 실제로 그 문제는 답안에 일부 이상이 있었고, 재채점 결과, 1-5위의 순위가 뒤집어지는 결과가 나오게 되었습니다. 채점 데이터를 제대로 검수하지 못한 탓이겠지요. 순위가 바뀌어 수상결과가 내려간 팀들에게는 진심으로 죄송하게 생각하고 있습니다.<br><br>
어떻게든 간에 대회가 끝났습니다. 제 생각대로 돌아간 부분도 있고, 제 생각대로 되지 않은 부분도 있습니다만, 전반적으로는 성공적이었던 것 같습니다. 대회 준비를 하며 문제를 풀었던 참가 학생들도 실력이 많이 늘었겠지만, 문제 출제와 서버 관리를 했던 저에게도 실력 신장의 시간이 되었던 것 같습니다. ~~그래서 보수는 얼마죠?~~ 앞으로도 HEPC가 좋은 문화로 남아 계속 개최되었으면 좋겠습니다. 물론, 제가 출제위원으로 참가하는 일은 다시는 없겠죠...?