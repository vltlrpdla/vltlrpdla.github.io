---
layout: post
title: http, https ?
date: 2018-06-03 18:32:20 +0300
description: secure web coding. # Add post description (optional)
img: secureweb.jpg # Add image post (optional)
tags: [third, post]
---

---
이번 05.19 topcit 시험에 http 관한 서술문제가 나왔는데 뭔가 답은 "https"다 하는 생각은 들지만 그 생각을 뒷받침 하는 근거를 도무지 서술할 수가 없었다. 사실 그 답은 컴퓨터 보안 시간에 교수님이 가르쳐 주었더라......

---  

### http(hyper text transfer protocol) ? https (s: over Secure socket layer) ?

**http** 란 _서버와 클라이언트간의 통신 규약_ 이라는 것을 웹 프로그래밍 시간에 배워 알고 있다. 그렇다면 https는 무엇일까 ?  
  
**https** 는  _TLS를 사용해 암호화된 연결을 하는 HTTP_ 이다.

 예전 교수님이 sha1이 나오는 강의를 할 때쯤 https에 대해서 언급한 적이 있다. 당시에 암호화와 복호화와 관계된 공개키에 대한 수업이었는데 역시 망각의 동물이라 머릿속에 남아있는건 그저 저런 키워드 뿐이다. 다음 포스트에서는 좀 더 자세하게 다뤄볼 예정이다.  
 

 
 <h3>TLS</h3> 
 
 나무위키의 도움을 받았다.
 
 >인터넷을 사용한 통신에서 보안을 확보하려면 두 통신 당사자가 서로가 신뢰할 수 있는 자임을 확인할 수 있어야 하며, 서로간의 통신 내용이 제3자에 의해 도청되는 것을 방지해야 한다. 따라서 서로 자신을 신뢰할 수 있음을 알리기 위해 전자 서명이 포함된 인증서를 사용하며, 도청을 방지하기 위해 통신 내용을 암호화한다. 이러한 통신 규약을 묶어 정리한 것이 바로 TLS. 주요 웹브라우저 주소창에 자물쇠 아이콘이 뜨는 것으로 TLS의 적용 여부를 확인할 수 있다

위에서 본 것과 같이 https는 암호화가 전혀 되어있지 않은 http의 프로토콜의 개선안이라고 보면 된다. 

둘의 기본적인 차이점은.
* URI의 차이 __http://__ vs __https://__
* port number  __http__ : __80__ / __https__ : __443__
* 암호화의 여부 __TLS__ __SSL__

---  

아무래도 추가적인 암호화의 과정을 거치기 때문에 다소 복잡하고 시간이 더 걸린다는 점, 세션을 통한 인증이기 때문에 인터넷 연결과 관련된다는 점을 제외한다면 요즘 대부분의 사람들이 인터넷을 통해 대화와 데이터 관리를 하고 있기 때문에 조금 번거롭지만, 개인 정보나 정보 보안에 대해 민감한 데이터를 다루는 곳에서는 필수적이라고 생각한다.

---