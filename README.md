# bgColor
the parsing process of 'bgcolor', a attribute of body tag.
exp:   bgcolor = 'bluegreen';
       css 解析成'b00，e00，ee0';
       非十六进制数用0代替；
       不为3的倍数在后面添0；
       然后截取对应的前两位 b0  e0  ee ;
       组成新的 rgba( b0 , e0 , ee );
       即为浏览器渲染的颜色。
