To work with date & time as date object, we need to import datetime. Which has year,month, date ,hour , minute,second and millisecond.

Date Output
If we want to display current time
			import datetime
			x = datetime.datetime.now() 
			print(x) 
	# which displays current time 
	Eg: 2020-08-01 13:06:50.990519 (YYYY-MM-DD HH:MM:SS:ms)

If we need Year and Name of weekday
			import datetime
			x = datetime.datetime.now()
			print(x.year) # which displays as 2020
			print(x.strftime("%A")) # which displays Saturday
			
Creating Date Objects
		If we want to construct date, we can use datetime() along with datetime module
Eg:		import datetime
			x = datetime.datetime(2020, 5, 17) # which displays 2020-05-17 00:00:00
			print(x)

 The Strftime() Method	
			The strftime() takes one parameter , format and return with string.
Eg:		import datetime
			x = datetime.datetime(2018, 6, 1)
			print(x.strftime("%B")) #%B directive are to find month name in full format
		#which display month name in full format as June


List of directories and Description
	


Directive
Description
Example
%a
Weekday, short version
Wed
%A
Weekday, full version
Wednesday
%w
Weekday as a number 0-6, 0 is Sunday
3
%d
Day of month 01-31
31
%b
Month name, short version
Dec
%B
Month name, full version
December
%m
Month as a number 01-12
12
%y
Year, short version, without century
18
%Y
Year, full version
2018
%H
Hour 00-23
17
%I
Hour 00-12
05
%p
AM/PM
PM
%M
Minute 00-59
41
%S
Second 00-59
08
%f
Microsecond 000000-999999
548513
%z
UTC offset
+0100
%Z
Timezone
CST
%j
Day number of year 001-366
365
%U
Week number of year, Sunday as the first day of week, 00-53
52
%W
Week number of year, Monday as the first day of week, 00-53
52
%c
Local version of date and time
Mon Dec 31 17:41:00 2018
%x
Local version of date
12/31/18
%X
Local version of time
17:41:00
%%
A % character
%


