# helloGitHub

## MarkDown的使用
1. 标题
# 标题
## 标题1
### 标题2
#### ...  
###### 标题6  

2. 有序无序列表
- 文本
- 文本
- 文本
1. 文本
2. 文本
3. 文本  
3. 超链接与图片
[百度](https://www.baidu.com/)
![](http://pic38.nipic.com/20140217/2531170_083242161000_2.jpg)  
4. 应用
> 密码密码木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木木
5. 斜体和粗体
*斜体* **粗体**
6. 代码应用
`private SurveyDaoImpl surveyDao;`
```
/**
 * 	新建调查
 */
	@Override
	public Survey newSurvey(User u) {
		Survey survey = new Survey();
		Page page = new Page();
//		关系关联
		page.setSurvey(survey);
		survey.getPages().add(page);
		survey.setUser(u);
//		数据库保存
		surveyDao.sayeEntity(survey);
		pageDao.sayeEntity(page);
		return survey;
	}
	
```  
7. 表格

dog | bird | cat
----|------|----
foo | foo  | foo
bar | bar  | bar
baz | baz  | baz  

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

