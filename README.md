# localStorage-sessionStorage-session

## localStorage
1. localStorage 只保存在客户端(不与服务器交互),永久保存(除非手动删除)，即使浏览器页面关闭，但是当再次打开页面(相同域名的其它页面，比如在index.html存入，然后关闭，再打开second.html仍然有存储信息)时，存储信息仍然存在，前提是域名相同，不能跨浏览器;
2. localStorage.setItem(key,value),key和value都是以字符串形式存在,localStorage.getItem(key)获取;localStorage.remove(key)删除某项;localStorage.clear()删除全部;
3. 存储空间比cookie要大;存储空间5M;
## sessionStorage
1. sessionStorage 只保存在客户端(不与服务器交互),当页面关闭时，存储信息也清除,当打开index.html页面时，通过页面跳转进入second.html，那么此时sessionStorage可以获取，如果单独进入second.html则sessionStorage不存在,但是localStorage却存在;存储空间5M；

## cookie 
1. cookie存在客户端(与服务器交互),可以设置存储时间，在index.html页面中设置cookie，那么在其他页面也可以获取到;存储空间4k;
# 三者跨浏览器都不可读取;