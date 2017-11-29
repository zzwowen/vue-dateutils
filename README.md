
[support] https://github.com/zzwowen/vue-dateutils

[bugs] https://github.com/zzwowen/vue-dateutils/issues

[npm] 

	npm install vue-dateutils

	cnpm install vue-dateutils --save

[script] 

	<script type="text/javascript" src="dateUtils.js"></script> 

	<script type="text/javascript" src="dateUtils.min.js"></script>

[Use]

	If you use NPM to introduce 'npm install vue-dateutils';

	import dateUtils from 'vue-dateutils';

	console.log(dateUtils.dateToStr("YYYY-MM-DD",new Date()));

	==>'2017-11-29'

	If you use the script label '<script type="text/javascript" src="dateUtils.min.js"></script>'

	console.log(dateUtils.dateToStr("YYYY-MM-DD",new Date()));

	==>'2017-11-29'

[method]

	/**
	 *Determine whether a date object is a leap year
	 *判断闰年
	 *param date (Date Object)
	 *return boolean true or false
	 */
===> isLeapYear(date)


 	/**
 	 *date to string
	 * 日期对象转换为指定格式的字符串
	 * @param f 日期格式,格式定义如下 yyyy-MM-dd HH:mm:ss
	 * @param date Date日期对象, 如果缺省，则为当前时间
	 *
	 * YYYY/yyyy/YY/yy 表示年份
	 * MM/M 月份
	 * W/w 星期
	 * dd/DD/d/D 日期
	 * hh/HH/h/H 时间
	 * mm/m 分钟
	 * ss/SS/s/S 秒
	 * @return string 指定格式的时间字符串
	 */
===>  dateToStr(format,date)


	/**
	 * calc date
	 * 日期计算
	 * @param strInterval string  可选值 y 年 m月 d日 w星期 ww周 h时 n分 s秒
	 * @param num int
	 * @param date Date 日期对象
	 * @return Date 返回日期对象
	 */
===>  dateAdd(strInterval, num, date)



	/**
	 *time difference
	 * 比较日期差 dtEnd 格式为日期型或者有效日期格式字符串
	 * @param strInterval string  可选值 y 年 m月 d日 w星期 ww周 h时 n分 s秒
	 * @param dtStart Date  可选值 y 年 m月 d日 w星期 ww周 h时 n分 s秒
	 * @param dtEnd Date  可选值 y 年 m月 d日 w星期 ww周 h时 n分 s秒
	 */
===>  dateDiff(strInterval, dtStart, dtEnd)


	/**
	 * string to date
	 * 字符串转换为日期对象
	 * @param date Date 格式为yyyy-MM-dd HH:mm:ss，必须按年月日时分秒的顺序，中间分隔符不限制
	 */
===> strToDate(dateStr)

	/**
	 * 把指定格式的字符串转换为日期对象yyyy-MM-dd HH:mm:ss
	 *
	 */
===> strFormatToDate(formatStr, dateStr)


	/**
	 * 日期对象转换为毫秒数
	 */
===> dateToLong(date)


	/**
	 * 毫秒转换为日期对象
	 * @param dateVal number 日期的毫秒数
	 */
===> longToDate(dateVal)


	/**
	 * 判断字符串是否为日期格式
	 * @param str string 字符串
	 * @param formatStr string 日期格式， 如下 yyyy-MM-dd
	 */
===> isDate(str, formatStr)



	/**
	  *当前年月的天数
	  */
===> getMaxDay(year, month)


	/**
	 * 把日期分割成数组 [年、月、日、时、分、秒]
	 */
===> toArray(myDate) 


	/**
	 * 取得日期数据信息
	 * 参数 interval 表示数据类型
	 * y 年 M月 d日 w星期 ww周 h时 n分 s秒
	 */
===>datePart(interval, myDate)


	/**
	 * 取得当前日期所在月的最大天数
	 */
===>maxDayOfDate(date)