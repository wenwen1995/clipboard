# clipboard
使用clipboard.js实现页面内容复制到剪贴板

具体的内容可以去github官网看，并下载相关用例。链接：[https://github.com/zenorocha/clipboard.js](https://github.com/zenorocha/clipboard.js)

步骤分为三步，

第一步，下载clipboard.min.js,在页面引入(先要引入jquery文件)

    <script type="text/javascript" src="../j/jquery-3.1.1.min.js"></script>
    <script type="text/javascript" src="../j/clipboard.js"></script>

第二步，在script标签里实例化语句

    <script type="text/javascript">  
        $(document).ready(function(){  
            var clipboard = new Clipboard('.btn');  
	}  
	</script>  

第三步，写页面按钮，实现点击按钮复制指定内容

     <input id="foo" value="https://github.com/zenorocha/clipboard.js.git">
    
     <!-- Trigger -->
      <button class="inputBtn" data-clipboard-target="#foo">copy</button>

