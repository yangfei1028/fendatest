# fendatest
1、测试集合单独建立一个目录，在FDTestCases目录下建立一个子目录存放相关的测试用例集合

2、相同页面或性质的测试用例放同一个目录
	
3、测试用例都以FDxxx开头，第一个字母大写
4、测试用例类名与测试文件名相同
5、每个测试用例都需要调用 init_case 方法，主要用于处理开屏广告或启动分答的时候的特殊情况
6、每条测试用例方法都以 test_xxx 开头
7、每条测试用例都开始都 print 一下测试方法的名字
8、每条测试用例最后都以回到热门页面为结束点
9、每条操作都标记注释
10、新建一个同测试文件名相同的txt文件，写下每条测试用例概况（参考：settingPage/MPsetting.txt 文件）
11、每条测试用例都标记作者如： #Edit by xxx 2017/7/12#
12、每条用例都要用try...except... 包起来，并调用截图模块
