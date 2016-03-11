###css 默认样式
css reset 都是什么样的都有
什么是默认样式
个人觉得在各类网站下都不会影响他们代码的  base 才算是默认样式
下面来一段个人一直用的

## base
	body, textarea, input, select, option {
	  font-size: 12px;
	  color: #333;
	  font-family: "Hiragino Sans GB", "Microsoft Yahei", tahoma, arial, sans-serif;
	  -webkit-font-smoothing: antialiased;
	}
	h1, h2, h3, h4, h5, h6 {
	  font-size: 100%;
	}
	body, h1, h2, h3, h4, h5, h6, blockquote, ol, ul, dl, dd, p, textarea, input, select, option, form {
	  margin: 0;
	}
	ol, ul, textarea, input, option, th, td {
	  padding: 0;
	}
	table {
	  border-collapse: collapse;
	}
	li {
	  list-style-type: none;
	}
	article, aside, details, figcaption, figure, footer, header, menu, nav, section {
	  display: block;
	}
	.cfix:after {content:'.';display:block;height:0;clear:both;visibility:hidden;}
	.cfix {*zoom:1;}
	.clear {
	  clear: both;
	  height: 0;
	  overflow: hidden;
	}
	a {
	  text-decoration: none;
	  color: #333;
	}
	a, textarea, input, select {
	  outline: none;
	}
	textarea {
	  overflow: auto;
	  resize: none;
	}
	.img img {
	  display: block;
	}
	a img {
	  border: none;
	}
	//.z-index {
	//  position: fixed;
	//  _position: absolute;
	//  z-index: 999;
	//  display: none;
	//  overflow: hidden;
	//}
	.pr {
	  position: relative;
	}
	.pa {
	  position: absolute;
	}
	.fl {
	  float: left;
	}
	.fr {
	  float: right;
	}
	a:hover {
	  text-decoration: underline;
	}
## 自定义
	.m {
	  margin: 0 auto;
	  width: 1200px;
	}
	.t10 {
	  margin-top: 10px;
	}
	.hide {
	  display: none;
	}
	.show {
	  display: block;
	}
	/**
	去ie10 小X
	*/
	::-ms-clear { display: none;}
	::-ms-reveal { display: none;}
	/**
	 placeholder color更改
	*/
	::-webkit-input-placeholder { /* WebKit browsers */
	    color:#ccc;
	}
	:-moz-placeholder { /* Mozilla Firefox 4 to 18 */
	    color:#ccc;
	}
	::-moz-placeholder { /* Mozilla Firefox 19+ */
	    color:#ccc;
	}
	:-ms-input-placeholder { /* Internet Explorer 10+ */
	    color:#ccc;
	}
## 备注
有人说var em cite i b strong 等标签没有重置
其实原来我是加了的，但有个问题，如果这个网站有用户编辑部分，自己增加了粗体斜体大字号 因为你重定义了，那strong b 等就不起作用了