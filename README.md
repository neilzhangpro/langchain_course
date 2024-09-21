## AI Agent智能应用从0到1定制开发 
## AI Agent Intelligent Application Custom Development from 0 to 1
******
- 此代码为网课《AI Agent智能应用从0到1定制开发》的配套代码，需要注意本套代码建议与网课适配配合食用。
- This code for the online course <AI Agent Intelligent Applications from 0 to 1 custom development> supporting code, need to pay attention to this set of code is recommended with the online course adapted to work with consumption.
- 需要注意由于课程开发周期的原因，langchain版本跨越了3个大版本，部分代码会与视频演示有差别!
- Note that due to the course development cycle, the langchain version spans 3 major releases and some of the code will differ from the video demo!
- 课程地址：https://coding.imooc.com/class/822.html
- Course address: https://coding.imooc.com/class/822.html

### 为什么要更新代码?
### Why update the code?
*******

课程从开发到商家大约经历了2~3个月的时间，中间Langchain发了大版本，导致很多API失效或有了变化，所以需要更新(目前AI领域的所有框架发展都很快)。另外一个重要原因很多用户是初级用户，对于Python很不熟悉，导致卡在第一步的环境搭建上无法进行。故需要将演示代码进行整理和部分升级改变以适应改变，并照顾新手学员。
The course has gone through about 2~3 months from development to merchants, and Langchain has released a major version in the middle, resulting in many APIs being invalid or changing, so they need to be updated (at present, all frameworks in the AI field are developing rapidly). Another important reason is that many users are beginner users and are not familiar with Python, which makes them stuck in the first step of environment construction. Therefore, it is necessary to organize and partially upgrade the demo code to adapt to the changes, and take care of the novice students.

### 主要的变化？
### What is chaged?
*******

1. 将早期课程的依赖包从0.0 升级到0.1，基本上课程主体部分以langchain 0.1大版本为主，因为0.0版本里改的东西比较多了
2. 将代码按照依赖版本划分命名空间，隔离依赖包污染(下面有具体做法)
3. 针对已经改变的API和示例，做了适当修改
1. Upgrade the dependency package of the early course from 0.0 to 0.1, basically the main part of the course is based on the Langchain 0.1 major version, because there are more changes in the 0.0 version
2. Divide the code into namespaces according to dependency versions and isolate dependency package contamination (see how to do it below)
3. Appropriate changes have been made to the changed APIs and examples

### 如何使用？
### How to use it?
****

- 首先推荐你购买该视频课程
- 推荐环境:
```
# windows 平台
# visual code
# python 3.12.1 + venv
# 其他平台请自行测试！
```
- 在VScode中打开后，请首先打开终端，执行如下命令
```
python -m venv langchain_v0.1
langchain_v0.1\Scripts\activate
# 这样就建好了第一个虚拟空间
```
- 按照顺序访问，注意01~33依赖该环境，请先在0.1中安装依赖包
- 接着在终端中输入如下命令
```
python -m venv langchain_v0.2
langchain_v0.2\Scripts\activate
# 这样就建好了第二个虚拟空间
```
- 按照顺序访问，注意33~46依赖该环境，请先在33中安装依赖包

### 目录
### catelog
*****
1. [langchain helloWorld](01.ipynb)
2. [langchain 提示词模板](02.ipynb)
3. [langchain 示例选择器](03.ipynb)
4. [langchain Loader](04.ipynb)
5. [langchain OpenAI](05.ipynb)
6. [langchain 文档切割](06.ipynb)
7. [langchain LostInTheMiddle](07.ipynb)
8. [langchain 嵌入向量](08.ipynb)
9. [langchain ChatDoc01](09.ipynb)
10. [langchain ChatDoc02](10.ipynb)
11. [langchain Chains](11.ipynb)
12. [langchain Load Chains](12.ipynb)
13. [langchain 文档链](13.ipynb)
14. [langchain 文档链](14.ipynb)
15. [langchain Memory](15.ipynb)
16. [langchain Memory on Chain](16.ipynb)
17. [langchain Clone a ChatGPT](17.ipynb)
18. [langchain Agent](18.ipynb)
19. [langchain Agent Types](19.ipynb)
20. [langchain Agent Memory](20.ipynb)
21. [langchain Tools](21.ipynb)
22. [langchain Toolkit](22.ipynb)
23. [langchain Custom Agent](23.ipynb)
24. [langchain LCEL](24.ipynb)
25. [langchain LCEL接口](25.ipynb)
26. [langchain LCEL提示词模版](26.ipynb)
27. [langchain Rnnable协议](27.ipynb)
28. [langchain LCEL Memory](28.ipynb)
29. [langchain LCEL Agent](29.ipynb)
30. [langchain 最佳实践](30.ipynb)
31. [langchain 版本说明](31.ipynb)
32. [langchain 接入通义千问](32.ipynb)
33. [langchainv0.2 接入智谱](33.ipynb)
34. [langchainv0.2 接入月之暗面](34.ipynb)
35. [langchainv0.2 接入百川智能](35.ipynb)
36. [langchainv0.2 流式事件支持](36.ipynb)
37. [langchainv0.2 @Chain修饰符](37.ipynb)
38. [langchainv0.2 工具调用](38.ipynb)
39. [langchainv0.2 返回结构化数据](39.ipynb)
40. [LangGraph HelloWorld](40.ipynb)
41. [LangGraph 持久化](41.ipynb)
42. [LangGraph 时光旅行](42.ipynb)
43. [LangGraph 流和异步](43.ipynb)
44. [LangGraph 图的可视化](44.ipynb)
45. [LangGraph 主从多Agents](45.ipynb)
46. [LangGraph 工作流配置](46.ipynb)
47. [LangGraph 双Agents](47.ipynb)

### 【如果你喜欢本课程】
### 【if you like the course】
*****

- 请购买课程: https://coding.imooc.com/class/822.html
- 请在课程评价页面给我打好评，这对于我至关重要!
- 请为这个仓库打个start★,这会帮助更多人找到资源!
- 请收藏或者分享我的AI笔记网站给需要的朋友: https://www.1goto.ai/