# JSTL, JSP 변수 공유

1. JSTL변수 JSP에서 사용

 <c:set var="test" value="테스트" />
 <%
      String test = (String)pageContext.getAttribute("test") ;
 %>


 2. JSP 변수 JSTL에서 사용

<%
      String test = "테스트" ;
      pageContext.setAttribute("test", test) ;
 %>

 <c:out value="${test}" />

 자료 출처 : https://intro0517.tistory.com/129