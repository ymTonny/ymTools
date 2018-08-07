//=======数组操作调用方式(支持链式调用)====//
arr.方法名 (数组对象排序采用:arr.sort(方法名)) arr为自己的数组变量
| 名称                   |功能                    |参数                                          |
| :----------------------|:----------------------|:---------------------------------------------|
| orderBy                |数组排序                |(rule) rule:'asc','desc'                      |
| compare                |数组对象排序            | (prop) prop:对象属性名(必须为数字形字符串)       |
| unique                 |数组去重（新数组）       |                                               |
| unique1                |数组去重（原数组）       |                                               |
| unique2                |数组对象去重(根据对象名)  |(键名)                                         |
| remove                 |删除数组中元素           |name                                           |
| removeObject           |删除数组对象中的元素      |键值                                           |
| arrMax                 |数组最大值(number型)     |                                               |
| arrMin                 |数组最小值(number型)     |                                               |
| arrRand                |数组随机排列             |                                               |
| arrRand1               |数组随机排序             |                                               |
| randItem               |数组随机取一个数据(包含undefind)                                          |
| isRepeat               |数组是否有重复项          |                                              |
| filterItem             |数组模糊过滤搜索          |query(模糊值)                                  |
//======日期操作调用方式======//
ymDate.方法名()    _dateAd函数返回(yyyy-mm-dd  hh:mm:ss)
|_transferDate           |日期"-"转为"/"           |date(string类型)                               |
|_numYear                |日期相差年份             |(date1,date2)  date1<date2                     |
|_numDay                 |日期相差天数             |(date1,date2)  date1<date2                     |
|_numHour                |日期相差小时             |(date1,date2)  date1<date2                     |
|_numMinute              |日期相差分钟             |(date1,date2)  date1<date2                     |
|_numSeconed             |日期相差秒数             |(date1,date2)  date1<date2                     |
|_numMillSecond          |日期相差毫秒数           |(date1,date2)  date1<date2                     |
|_dateAdMSecond          |日期加(减)上毫秒数        |(date,millsecond,Operator) Operator:"ad"(加) "cut"(减)|
|_dateAdSecond           |日期加(减)上秒数          |(date,second,Operator)同上                     |
|_dateAdMinute           |日期加(减)上分钟          |(date,minute,Operator)同上                     |
|_dateAdHours            |日期加(减)上小时          |(date,hours,Operator)同上                      |
|_dateAdDay              |日期加(减)上天            |(date,day,Operator)同上                        |
|_dateAdMonth            |日期加(减)上月(30,31已计算)|(date,month，Operator)同上                     |
|_dateAdYear             |日期加(减)上年            |(date,year,loop,Operator) loop(true按闰年)同上  |
|_getDayWeek             |日期在当月星期几           |(date) 返回(1,2,3,4,5,6,0)                     |
|_getWeekCh              |日期在当月星期几           |(date) 返回("星期日",......)                    |
//=========文件操作调用方式=======//
ymFile.方法名（）
|fileExt                 |获取文件后缀名             |(fileName)                                    |
|getfileName             |获取文件名(去后缀)         |(fileName)                                    |
|filterHTML              |将html转成字符串输出       |(str) "<p></p>"                               |
|cardID                  |身份证号验证               |(code)"身份证号"                              |
|numberCh                |数字转为中文               |(number)                                     |
|numberMoney             |数字转为对应大写金额        |(number||string)                             |
|DrawImage               |图片等比例缩放             |(ImgD,maxwidth,maxheight)ImgD:图片对象        |
//=========浏览器操作调用方式=====//
ymURL.方法名()
|getURLParam             |获取浏览器url中的参数值     |(url)                                        |
|isBrowser               |判断当前浏览器类型          |                                             |
//=========常规正则验证调用方式=======//
ymregRule.方法名(val)
|email                   |验证邮箱                   |val                                          |
|userName                |验证用户名(3-16英文字母或数字)|val                                         |
|chineseName             |验证中文姓名                |val                                         |
|mobile                  |验证手机号码                |val                                         |
|tel                     |验证固定电话                |val                                         |
|idCard                  |验证身份证                  |val                                         |
|amount                  |验证金额为两位小数           |val                                         |
|positiveInt             |验证正整数                  |val                                         |
|int                     |验证整数(不限位数)           |val                                         |
|bankCard                |验证16或19位银行卡号         |val                                         |
|chinese                 |验证是否是中文               |val                                         |
|decimalNumber           |验证带小数的数字             |val                                         |
|ip                      |验证ip                      |val                                         |
//==========元素节点调用方式==========//
ymElement.方法名()    元素移动匀速移动请设置默认transtion top:0 left:0
|getStyle                |获取元素样式                 |(elem,prop)elem:节点,prop:样式名             |
|elemMove                |元素左右或上下运动            |(elem,dir,time,long,callback)dir:方向("top","left"),long:移动距离|