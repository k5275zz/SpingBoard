# SpingBoard

<h3>게시판 글쓰기, 리스트, 상세페이지, 수정 및 삭제</h3>
<hr>
<p>DTO : <i>변수를 담고 넘겨주는 역활 (bean)</i> <br>
DAO.java,DAO.xml : sql문 로직을 실행 (model)<br>
Service, ServiceImpl : model > Service를 거쳐 처리한다. Tier3방식을 이용해 메소드를 한번 더 거쳐 보안성이 좋아진다.<br>
write.jsp : 글쓰기 페이지<br>
list.jsp : 글목록 페이지<br>
detail.jsp : 상세정보페이지<br></p>


<br>

![image](https://user-images.githubusercontent.com/71121027/100572833-cf4c1180-3319-11eb-9c2b-6bc12d53990d.png)

<b>글쓰기 등록 시 컨트롤러를 통해 글이 등록되고 전체 글목록 페이지(list.jsp)로 이동한다.</b>

<br>

<hr>

![image](https://user-images.githubusercontent.com/71121027/100572951-14704380-331a-11eb-9731-03d37f05f53b.png)

<b>전글에서 만든 list.jsp에서 게시물번호(bno)에 하이퍼링크를 걸고 게시물번호(bno)를 클릭하면 클릭한 bno에 대한 상세페이지(detail.jsp)가 나온다.</b>

<b>하이퍼링크에 ?bno=${}를 추가해서 클릭한 글의 기본키 값인 게시물번호(bno)를 넘겨준다.</b>

<br>

<hr>

![image](https://user-images.githubusercontent.com/71121027/100572979-24882300-331a-11eb-9f97-8b3d6527c193.png)

<b>받아온 게시물번호(bno)에 맞는 글을 삭제 또는 수정한다.</b>
