目录  
[标题](# 标题)  
[列表](# 列表)  

# 标题
标题可以使用`#`来标注
>`# 一级标题`  
>`## 二级标题`  
>`### 三级标题`  
>`#### 四级标题`  
>`##### 五级标题`  
>`###### 六级标题`

**效果展示**
# 一级标题  
## 二级标题  
### 三级标题  
#### 四级标题  
##### 五级标题  
###### 六级标题

# 列表
列表可以使用`+`,`-`,`*`,`1,2,3...`来表示
>`+ 列表1`  
>`+ 列表2`  
>`- 列表1`  
>`- 列表2`  
>`* 列表1`  
>`* 列表2`  
>`1 列表1`  
>`2 列表2`  

**效果展示**
+ 列表1
+ 列表2  

1 列表1  
2 列表2  

github 支持任务列表模式  
- [ ] 表示待做`- [ ] `  
- [X] 表示已经完成`- [ X ] `    

# 段落
段落的前后需要有空行，如果要强制换行则需要连续两个以上空格加换行

# 分割线
markdown中的分割线可以使用三个连续的\***, \--- 来表示  

---
***

# 引用
引用一般使用`>`在每行开始处标记，可以嵌套使用  
**效果展示**  
> line1  
> line2  
> line3  
>> line4    

# 代码块
代码块可以使用\` \`或者\``` \```来使用  
* \` \` 表示的是行内代码  
* \``` \``` 则表示的是一个代码块,如果要高亮代码需要在前面的三个\```后面加上语言名字，例如python, rust等  

这里是代码块  
```python
import re  
sa = re.compile(r'\w+@\w+\.com')  
m = sa.match('hugowu@163.com')  
print(m.groups())
```

# 强调
+ 使用`**强调**` 表示**强调**    
+ 使用`*斜体*` 表示*斜体*
+ 使用`*你**可以**强调他们* `表示*你**可以**强调他们*  
+ 使用`~~删除线~~`表示~~删除线~~

# 图片
![baidu](http://www.baidu.com/img/bdlogo.gif '百度')

# 链接
+ 行内式  
`[anuowu的Markdown库](https://github.com/anuowu/productive_tools)`  
**效果**  
[anuowu的Markdown库](https://github.com/anuowu/productive_tools)  
+ 参考式  
`[anuowu的Markdown库][1]`  
`[1]:(https://github.com/anuowu/productive_tools)`  
**效果**  
[anuowu的Markdown库][1]  
[1]:(https://github.com/anuowu/productive_tools)  

# 表格
>`first header | second header | third header`  
>`-------------| ------------- | ----------- `   
>`content cell | content cell  | content cell`    
>`content cell | content cell  | content cell`  

**效果**  

first header | second header | third header   
------------ | ------------- | -----------  
content cell | content cell  | content cell  
content cell | content cell  | content cell  

表格对齐  
>`first header | second header | third header`  
>`:------------| :-----------: | -----------:`   
>`content cell | content cell  | content cell`    
>`content cell | content cell  | content cell`  

**效果**  

first header   |   second header   |   third header     
:-----------   |   :----------:    |   ----------:  
content cell   |   content cell    |   content cell    
content cell   |   content cell    |   content cell    

# 表情
github 支持 markdown 语法的表情  
 :bowtie: :joy: :stuck_out_tongue_closed_eyes:
可以从[https://www.webpagefx.com/tools/emoji-cheat-sheet/](https://www.webpagefx.com/tools/emoji-cheat-sheet/)发现更多的表情
