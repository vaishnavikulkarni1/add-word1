<%-- 
    Document   : addword1
    Created on : Feb 24, 2019, 3:00:19 PM
    Author     : Abhiram
--%>

<%@page import="java.sql.Statement"%>
<%@page import="java.sql.ResultSet"%>
<%@page import="java.io.*"%>
<%
String word=request.getParameter("bword");
String word1="\n"+word;
//BufferedOutputStream bw=new BufferedOutputStream(new FileOutputStream("D:\\project\\new code1\\new code\\find.txt",true));
FileWriter fw=new FileWriter("F:\\javatest\\socialNetwork\\find1.txt",true);
fw.write("\r\n"+word);
fw.close();
response.sendRedirect("adminuser.jsp?m=done");

%>
