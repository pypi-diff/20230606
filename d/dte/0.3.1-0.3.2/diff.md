# Comparing `tmp/dte-0.3.1.tar.gz` & `tmp/dte-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dte-0.3.1.tar", last modified: Tue Dec  7 22:24:55 2021, max compression
+gzip compressed data, was "dte-0.3.2.tar", last modified: Tue Jun  6 02:00:59 2023, max compression
```

## Comparing `dte-0.3.1.tar` & `dte-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-07 22:24:55.679005 dte-0.3.1/
--rwxrwxrwx   0 root         (0) root         (0)      464 2021-01-20 02:30:16.000000 dte-0.3.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     9390 2021-12-07 22:24:55.678563 dte-0.3.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     8723 2021-12-07 22:23:33.000000 dte-0.3.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-07 22:24:55.674037 dte-0.3.1/dte/
--rwxrwxrwx   0 root         (0) root         (0)    40398 2021-12-07 22:24:18.000000 dte-0.3.1/dte/dte
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-07 22:24:55.677057 dte-0.3.1/dte.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     9390 2021-12-07 22:24:53.000000 dte-0.3.1/dte.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      181 2021-12-07 22:24:53.000000 dte-0.3.1/dte.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-12-07 22:24:53.000000 dte-0.3.1/dte.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       28 2021-12-07 22:24:53.000000 dte-0.3.1/dte.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-12-07 22:24:53.000000 dte-0.3.1/dte.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2021-12-07 22:24:55.679161 dte-0.3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1026 2021-12-07 22:24:53.000000 dte-0.3.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-07 22:24:55.677473 dte-0.3.1/test/
--rwxrwxrwx   0 root         (0) root         (0)    15866 2021-12-07 22:23:04.000000 dte-0.3.1/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 02:00:59.366148 dte-0.3.2/
+-rwxrwxrwx   0 root         (0) root         (0)      464 2021-01-20 02:30:16.000000 dte-0.3.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     8418 2023-06-06 02:00:59.365239 dte-0.3.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7686 2023-06-06 01:54:31.000000 dte-0.3.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 02:00:59.336310 dte-0.3.2/dte/
+-rwxrwxrwx   0 root         (0) root         (0)    40409 2023-06-06 01:53:36.000000 dte-0.3.2/dte/dte
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 02:00:59.345007 dte-0.3.2/dte.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     8418 2023-06-06 02:00:58.000000 dte-0.3.2/dte.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      181 2023-06-06 02:00:59.000000 dte-0.3.2/dte.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-06 02:00:58.000000 dte-0.3.2/dte.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       28 2023-06-06 02:00:58.000000 dte-0.3.2/dte.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-06 02:00:58.000000 dte-0.3.2/dte.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-06 02:00:59.366352 dte-0.3.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1128 2023-06-06 02:00:55.000000 dte-0.3.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 02:00:59.346245 dte-0.3.2/test/
+-rwxrwxrwx   0 root         (0) root         (0)    15940 2021-12-17 22:44:16.000000 dte-0.3.2/test/test.py
```

### Comparing `dte-0.3.1/dte/dte` & `dte-0.3.2/dte/dte`

 * *Files 2% similar despite different names*

```diff
@@ -284,23 +284,23 @@
 t_RPAREN = r'\)'
 t_GT = r'>'
 t_GE = r'>='
 t_LT = r'<'
 t_LE = r'<='
 t_EQ = r'=='
 t_NE = r'!='
-t_IN = r'(?i)in'
-t_UNTIL = r'(?i)until'
-t_SINCE = r'(?i)since'
-t_WAIT = r'(?i)wait'
-t_MONTH_LITERAL = r'(?i)month'
-t_WEEKDAY_LITERAL = r'(?i)weekday'
-t_OR = '(?i)or'
-t_AND = '(?i)and'
-t_TO = '(?i)to'
+t_IN = r'(?i:in)'
+t_UNTIL = r'(?i:until)'
+t_SINCE = r'(?i:since)'
+t_WAIT = r'(?i:wait)'
+t_MONTH_LITERAL = r'(?i:month)'
+t_WEEKDAY_LITERAL = r'(?i:weekday)'
+t_OR = '(?i:or)'
+t_AND = '(?i:and)'
+t_TO = '(?i:to)'
 
 reserved = [
             r'in',
             r'next|last',
             r'seconds|minutes|hours|days|weeks',
             r'wait',
             r'until',
@@ -325,21 +325,21 @@
 REGEX_DOY = r'(\d+(?!:)(?:\W)\d+(?!:)(?:\W)\d+|\d+[\W\s]+(?:' + \
         REGEX_ALL_MONTHS + \
         r')(?:\s|[^\w\+])+\d+)(?:st|nd|rd|th)?'
 REGEX_0_23 = r'(2[0-3]|1?[0-9]|00)'
 REGEX_0_59 = r'([0-5]?[0-9])'
 
 DATETIME_REGEX = \
-    fr'(?i)(?:{REGEX_DOY}\s?|' + \
+    fr'(?i:(?:{REGEX_DOY}\s?|' + \
     r'(?:(1[0-2]|[0-9])\s*([aApP][mM])|' + \
     fr'{REGEX_0_59}([hHm])?' + \
     f'(?::{REGEX_0_59}([msS])?' + \
     f'(?::(?:{REGEX_0_59}([sS])?))?' + \
     r'))(?:\s*([aApP][mM]))?' + \
-    '){1,2}'
+    '){1,2})'
 
 @TOKEN(DATETIME_REGEX)
 def t_DATETIME(t):
     date_str,\
         zeroth_val,\
         zeroth_ampm,\
         first_val,\
@@ -484,19 +484,19 @@
 # @TOKEN(_NAME)
 # def t_NAME(t):
 #     return t
 
 
 REGEX_1_12 = '(1[0-2]|[1-9])'
 REGEX_1_12_OPTIONALLY_PADDED = '(1[0-2]|0?[0-9])'
-BASEDATE_REGEX = r'(?i)(?:' + \
+BASEDATE_REGEX = r'(?i:(?:' + \
         r'('+REGEX_ALL_MONTHS+r')(?!:|\+|;)\W+(\d+)|' + \
         r'(\d+)(?!:|\+|;)\W('+REGEX_ALL_MONTHS+')|' + \
         r'(\d+)(?!:|\+|;)\W'+REGEX_1_12_OPTIONALLY_PADDED + \
-        ')'
+        '))'
 
 @TOKEN(BASEDATE_REGEX)
 def t_BASEDATE(t):
     m1, y1, y2, m2, y3, m3 = re.search(BASEDATE_REGEX, t.value).groups()
     if m1:
         month = m1
         year = y1
@@ -511,29 +511,29 @@
     if not month_index:
         month_index = int(month)
     t.value = Basedate(year, month_index)
     return t
 
 
 def t_UNIT(t):
-    r'(?i)(seconds|minutes|hours|days|weeks|months|years|unix)'
+    r'(?i:seconds|minutes|hours|days|weeks|months|years|unix)'
     return t
 
 
-WEEKDAY_TOKEN = r'(?i)Monday|Tuesday|Wednesday|Thursday|Friday|' + \
-    'Saturday|Sunday|Mon(?!th)|Tue|Wed|Thu|Fri|Sat|Sun'
+WEEKDAY_TOKEN = r'(?i:Monday|Tuesday|Wednesday|Thursday|Friday|' + \
+    'Saturday|Sunday|Mon(?!th)|Tue|Wed|Thu|Fri|Sat|Sun)'
 
 
 @TOKEN(WEEKDAY_TOKEN)
 def t_WEEKDAY(t):
     t.value = Weekday(t.value)
     return t
 
 
-@TOKEN(r'(?i)' + '|'.join(months) + '|'.join(months_abbrev))
+@TOKEN(r'(?i:' + '|'.join(months) + '|'.join(months_abbrev) + ')')
 def t_MONTH(t):
     t.value = Month(t.value)
     return t
 
 
 class Indexable(Enum):
     FIRST = 1
@@ -552,15 +552,15 @@
         Indexable.THIRD,
         Indexable.FOURTH,
         Indexable.FIFTH
         ]
 
 
 def t_INDEXABLE_OP(t):
-    r'(?i)(next|last|first|prev(ious)?|1st|2nd|3rd|4th|5th|first|second|third|fourth|fifth)'
+    r'(?i:(next|last|first|prev(ious)?|1st|2nd|3rd|4th|5th|first|second|third|fourth|fifth))'
     t.value = t.value.lower()
     if t.value.startswith('previous'):
         t.value = Indexable.PREVIOUS
     if t.value == 'next':
         t.value = Indexable.NEXT
     if t.value == 'last':
         t.value = Indexable.LAST
@@ -677,15 +677,15 @@
 lex.lex(debug=False)
 
 def wait(t):
     now = names['n']
     if isinstance(t, datetime):
         delta = t - now
     elif isinstance(t, date):
-        delta = t - now.date()
+        delta = datetime.combine(t, datetime.min.time()) - now
     elif isinstance(t, time):
         delta = datetime.combine(now.date(), t) - now
     elif isinstance(t, timedelta):
         delta = t
     else:
         print('Wait accepts a time point or time delta only', file=sys.stderr)
     if delta > timedelta(0):
@@ -741,15 +741,14 @@
 names = {
             'day': lambda t: t.day,
             'month': lambda t: t.month,
             'year': lambda t: t.year,
             'hour': lambda t: t.hour,
             'minute': lambda t: t.minute,
             'second': lambda t: t.second,
-            'wait': lambda t: wait(t),
             'weekday': lambda t: weekday(t),
             'dayofweek': lambda t: weekday(t),
             'help': lambda: print(HELP),
         }
 
 
 precedence = (
```

### Comparing `dte-0.3.1/setup.py` & `dte-0.3.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='dte',  
-     version='0.3.1',
+     version='0.3.2',
      author="Marcelo V. Rozanti",
      author_email="mvrozanti@hotmail.com",
      description="Date Time Expressions",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/mvrozanti/dte",
      packages=setuptools.find_packages('dte'),
@@ -25,10 +25,12 @@
          "Development Status :: 4 - Beta",
          "Topic :: Artistic Software",
          "Intended Audience :: Developers",
          "Programming Language :: Python :: 3.6",
          "Programming Language :: Python :: 3.7",
          "Programming Language :: Python :: 3.8",
          "Programming Language :: Python :: 3.9",
+         "Programming Language :: Python :: 3.10",
+         "Programming Language :: Python :: 3.11",
          "Programming Language :: Python :: 3 :: Only",
          ],
  )
```

### Comparing `dte-0.3.1/test/test.py` & `dte-0.3.2/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,190 +21,190 @@
 HMS_FORMAT = r'^\d+:\d+:\d+$'
 
 DELTA_FORMAT = r'(-?\d+ years?, (-?\d+ months?(, )?)? ?)?(-?\d+ days?, \d{1,2}:\d{2}:\d{2})?'
 
 BASEDATE_FORMAT = r'\d+-\w+'
 
 test_expectancy = OrderedDict({
-        '(T-1d).weekday'                        : lambda r: r in days,
-        '(n + 180d)-180d == n'                  : lambda r: eval(r),
-        '(n + 181d)-180d != n'                  : lambda r: eval(r),
-        '(t + 180d)-180d == t'                  : lambda r: eval(r),
-        '-1d.weekday'                           : lambda r: r in days,
-        '08h30'                                 : lambda r: r == '8:30:00',
-        '1 in unix'                             : lambda r: r == '1',
-        # '1m in hours'                           : lambda r: r == '1',
-        'n - 1234'                              : lambda r: re.match(DELTA_FORMAT, r),
-        '10h30 + 14h'                           : lambda r: r == '1 day, 0:30:00',
-        '2021 feb 14 12:00:00'                  : lambda r: r == '2021-02-14 12:00:00',
-        'seconds until 2021 feb 14 12:00:00'    : lambda r: float(r) < 580301.752936,
-        '1-1-1 23:23:23'                        : lambda r: re.match(ISO_FORMAT, r),
-        '1-1-1 23:23m'                          : lambda r: re.match(ISO_FORMAT, r),
-        '1-1-1 23h:23'                          : lambda r: re.match(ISO_FORMAT, r),
-        '1-1-1 23h:23m'                         : lambda r: re.match(ISO_FORMAT, r),
-        '1-1-1 23m:23'                          : lambda r: re.match(ISO_FORMAT, r),
-        '1-1-1 23m:23s'                         : lambda r: re.match(ISO_FORMAT, r),
-        '1-1-1 23m:23S'                         : lambda r: re.match(ISO_FORMAT, r),
-        '1-1-1 23:23S'                          : lambda r: re.match(ISO_FORMAT, r),
-        '11h:20 AM'                             : lambda r: r == '11:20:00',
-        '11m:20 PM'                             : lambda r: r == '00:11:20',
-        '11h:20 am'                             : lambda r: r == '11:20:00',
-        '11h:20m pm'                            : lambda r: r == '23:20:00',
-        '11:20s PM'                             : lambda r: r == '00:11:20',
-        '2014 Jan 13'                           : lambda r: r == '2014-01-13',
-        '2014 January 13'                       : lambda r: r == '2014-01-13',
-        '1996.04.28'                            : lambda r: r == '1996-04-28',
-        '22h:22'                                : lambda r: r == '22:22:00',
-        '22:22:22'                              : lambda r: r == '22:22:22',
-        '22h:22m:22'                            : lambda r: r == '22:22:22',
-        '22h:22m:22s'                           : lambda r: r == '22:22:22',
-        '22:22m:22s'                            : lambda r: r == '22:22:22',
-        '22h:22:22s'                            : lambda r: r == '22:22:22',
-        '22:22:22s'                             : lambda r: r == '22:22:22',
-        '22:22:22'                              : lambda r: re.match(HMS_FORMAT, r),
-        '2020-Jan-27'                           : lambda r: r == '2020-01-27',
-        '6 pm'                                  : lambda r: re.match(HMS_FORMAT, r),
-        '6 pm + 1h'                             : lambda r: re.match(HMS_FORMAT, r),
-        '6pm'                                   : lambda r: re.match(HMS_FORMAT, r),
-        '22m:22 + 4h'                           : lambda r: r == '4:22:22',
-        '1-1-1-1-1-1'                           : lambda r: '0:00:00',
-        '1610494238'                            : lambda r: '2021-01-12' in r,
-        '1610494238+4h.weekday'                 : lambda r: r == 'Wednesday',
-        '1610494238.weekday'                    : lambda r: r == 'Tuesday',
-        '12h:00 AM != 12h:00 PM'                : lambda r: eval(r),
-        '2014 Jan 13==2014 January 13'          : lambda r: eval(r),
-        '1957-12-26 - t'                        : lambda r: re.match(DELTA_FORMAT, r),
-        '1957-12-26 22:22:22 - t'               : lambda r: re.match(DELTA_FORMAT, r),
-        '1958-05-14 - 1958-05-16'               : lambda r: r == '-2 days, 0:00:00',
-        '1d in hours'                           : lambda r: r == '24.00',
-        '1d in minutes'                         : lambda r: r == '1440.00',
-        '1d in seconds'                         : lambda r: r == '86400.00',
-        '1d'                                    : lambda r: r == '1 day, 0:00:00',
-        '1d+0h22m'                              : lambda r: r == '1 day, 0:22:00',
-        '1d1m in hours'                         : lambda r: r == '24.02',
-        '1970 Jan 1 - 3h in unix'               : lambda r: int(r) <= 24*60*60,
-        '1w'                                    : lambda r: r == '7 days, 0:00:00',
-        '2020 Jan 27 + 1y == 2021 Jan 27'       : lambda r: eval(r),
-        '2 < 1'                                 : lambda r: not eval(r),
-        '12h:00 pm != 12h:00 am'                : lambda r: eval(r),
-        '22h+2m'                                : lambda r: r == '22:02:00', 
-        '22h22m'                                : lambda r: r == '22:22:00', 
-        '6y5M4d3h2m1s'                          : lambda r: re.match(DELTA_FORMAT, r),
-        '1y2M'                                  : lambda r: r == '1 year, 2 months',
-        '0y2M'                                  : lambda r: r == '2 months',
-        '-1y2M'                                 : lambda r: re.match(DELTA_FORMAT, r),
-        '1M1d'                                  : lambda r: r == '1 month, 1 day, 0:00:00',
-        '7y6M5w4d3h2m1.1s'                      : lambda r: re.match(DELTA_FORMAT, r),
-        '2h2m'                                  : lambda r: r == '2:02:00',
-        '3h+3M'                                 : lambda r: re.match(DELTA_FORMAT, r),
-        '3M'                                    : lambda r: re.match(DELTA_FORMAT, r),
-        'T-1.5d'                                : lambda r: re.match(ISO_FORMAT, r),
-        'T-10d'                                 : lambda r: re.match(YMD_FORMAT, r),
-        'T.day'                                 : lambda r: 0 < int(r) < 32,
-        'T.weekday'                             : lambda r: r in days,
-        'YD.day'                                : lambda r: re.match(r'\d+', r),
-        'n'                                     : lambda r: re.match(ISO_FORMAT, r),
-        'next Sunday'                           : lambda r: re.match(YMD_FORMAT, r),
-        '2000-10-10 00:16'                      : lambda r: r == '2000-10-10 00:16:00',
-        '2000-10-10 16:00'                      : lambda r: r == '2000-10-10 16:00:00',
-        'seconds until 3000 Apr 10'             : lambda r: 30899416627.60163 > float(r),
-        'seconds since 3000 Apr 10'             : lambda r: -30899416627.60163 < float(r),
-        'next Sunday == last sunday'            : lambda r: r == 'False',
-        'next Sunday != last sunday'            : lambda r: r == 'True',
-        'last Sunday == next sunday'            : lambda r: r == 'False',
-        'last Sunday != next sunday'            : lambda r: r == 'True',
-        'last sunday in 2021'                   : lambda r: r == '2021-12-26',
-        'first sunday in 2021'                  : lambda r: r == '2021-01-03',
-        '1st sunday in 2021'                    : lambda r: r == '2021-01-03',
-        '2012-12-13-3y.weekday'                 : lambda r: r == 'Sunday',
-        't - next Sunday'                       : lambda r: re.match(DELTA_FORMAT, r),
-        'wait .001s'                            : lambda r: len(r) == 0,
-        'wait until (n+.001s)'                  : lambda r: len(r) == 0,
-        'weekday 0'                             : lambda r: r in ['Wednesday', 'Thursday'],
-        'Jan 2014'                              : lambda r: re.match(BASEDATE_FORMAT, r),
-        'first friday in April 2014'            : lambda r: r == '2014-04-04',
-        '1st friday in April 2014'              : lambda r: r == '2014-04-04',
-        'first sun in April 2021'               : lambda r: r == '2021-04-04',
-        '1st sun in April 2021'                 : lambda r: r == '2021-04-04',
-        'yd-5h'                                 : lambda r: re.match(ISO_FORMAT, r),
-        '1957-12-26 22:22:22 in unix'           : lambda r: -379118258 - 86400 < int(r) < -379118258 + 86400,
-        '5m+5m'                                 : lambda r: r == '0:10:00',
-        '1h in seconds'                         : lambda r: r == '3600.00',
-        '1 hour in seconds'                     : lambda r: r == '3600.00',
-        '2s2s'                                  : lambda r: r == '0:00:04',
-        '1996 August 28 9 AM'                   : lambda r: r == '1996-08-28 09:00:00',
-        'seconds until tomorrow'                : lambda r: 0 < float(r) < 86400,
-        'seconds until 11 pm'                   : lambda r: float(r) < 86400,
-        'next month'                            : lambda r: re.match(BASEDATE_FORMAT, r),
-        'first friday in next month'            : lambda r: re.match(YMD_FORMAT, r),
-        '1st friday in next month'              : lambda r: re.match(YMD_FORMAT, r),
-        'first friday in april'                 : lambda r: re.match(YMD_FORMAT, r) and r.split('-')[1] == '04',
-        '1st friday in april'                   : lambda r: re.match(YMD_FORMAT, r) and r.split('-')[1] == '04',
-        '2014 01'                               : lambda r: re.match(BASEDATE_FORMAT, r), 
-        '6pm+1h'                                : lambda r: re.match(HMS_FORMAT, r),
-        'days until 2030-12-25'                 : lambda r: float(r) < 3364.55,
-        'last fri in 2014 December'             : lambda r: re.match(YMD_FORMAT, r),
-        'last fri in 2014 Dec'                  : lambda r: re.match(YMD_FORMAT, r),
-        'last fri in Dec 2014'                  : lambda r: re.match(YMD_FORMAT, r),
-        'yesterday==thursday'                   : lambda r: r in ['True', 'False'],
-        'yesterday==thu'                        : lambda r: r in ['True', 'False'],
-        'weekday tm'                            : lambda r: r in days,
-        '(weekday t+100d)'                      : lambda r: r in days,
-        '(weekday t+100d)==100d.weekday'        : lambda r: eval(r),
-        'weekday t+100d'                        : lambda r: r in days,
-        'monday+1d'                             : lambda r: re.match(YMD_FORMAT, r),
-        'next mon + 1d'                         : lambda r: re.match(YMD_FORMAT, r),
-        'days until next mon'                   : lambda r: 0 <= float(r) <= 7,
-        'days until mon'                        : lambda r: -4.5 < float(r) < 4.5,
-        'today==mon'                            : lambda r: r in ['True', 'False'],
-        'seconds in 24h'                        : lambda r: float(r) == 86400,
-        'Jan 2014 + 1M'                         : lambda r: re.match(YMD_FORMAT, r),
-        '2014 Jan + 1M'                         : lambda r: re.match(YMD_FORMAT, r),
-        '-1d + 2020-10-10'                      : lambda r: r == '2020-10-09',
-        '2nd sunday in 2021'                    : lambda r: r == '2021-01-10',
-        '3rd sunday in 2021'                    : lambda r: r == '2021-01-17',
-        '4th sunday in 2021'                    : lambda r: r == '2021-01-24',
-        '5th sunday in 2021'                    : lambda r: r == '2021-01-31',
-        '4th wed in august'                     : lambda r: re.match(YMD_FORMAT, r),
-        'august'                                : lambda r: re.match(BASEDATE_FORMAT, r),
-        't 1am'                                 : lambda r: re.match(ISO_FORMAT, r),
-        't 1:00'                                : lambda r: re.match(ISO_FORMAT, r),
-        't 1:00 == t 1am'                       : lambda r: eval(r),
-        '(2020-10-10+1d) 3pm'                   : lambda r: '2020-10-11 15:00:00' == r, 
-        '1am t'                                 : lambda r: re.match(ISO_FORMAT, r),
-        '1am t == t 1am'                        : lambda r: eval(r),
-        't+1d 08h30'                            : lambda r: re.match(ISO_FORMAT, r),
-        'april+1M'                              : lambda r: re.match(YMD_FORMAT, r),
-        'last sun in 2021'                      : lambda r: r == '2021-12-26',
-        'days until Jan 2030'                   : lambda r: float(r) < 3002,
-        '2020-01-29 + (1 year + 1 month)'       : lambda r: r == '2021-02-28',
-        'friday in 2015'                        : lambda r: re.match(YMD_LIST_FORMAT, r),
-        'fri in 2015'                           : lambda r: re.match(YMD_LIST_FORMAT, r),
-        'friday day 13 in 2015'                 : lambda r: re.match(YMD_LIST_FORMAT, r),
-        'friday day 13 in 2015.weekday'         : lambda r: re.match(DAY_LIST_FORMAT, r),
-        'friday day 13 in August 2021'          : lambda r: r == '2021-08-13',
-        'friday day 13 in August 2021.weekday'  : lambda r: r == 'Friday',
-        'friday day 13 in Jan 2015 to Jan 2019' : lambda r: re.match(YMD_LIST_FORMAT, r),
-        'friday day < 8 in Jan 2015 to Jan 2019': lambda r: re.match(YMD_LIST_FORMAT, r),
-        'friday day > 8 in Jan 2015 to Jan 2019': lambda r: re.match(YMD_LIST_FORMAT, r),
-        'friday day < 8 in Jan 2015'            : lambda r: r == '2015-01-02',
-        'friday in Jan 2015'                    : lambda r: re.match(YMD_LIST_FORMAT, r),
-        'friday day < 13 in 2014 sep'           : lambda r: re.match(YMD_LIST_FORMAT, r),
-        'day 13 friday in 2021'                 : lambda r: re.match(YMD_LIST_FORMAT, r),
-        '1970 january 1st'                      : lambda r: re.match(YMD_LIST_FORMAT, r), 
-        'jan 1 + 99999M'                        : lambda r: r.endswith('01')
-        # 'Jan 2014 3:00'                         : lambda r: False,
-        # '2014 Jan 3:00'                         : lambda r: False,
-
-        # 'friday day = 8 in Jan 2015' : lambda r: r == '2015-01-02',
-        # 'fris in 2015' # rrule
-        # 'fridays in 2015' # rrule
-        # 'easter 2014'                       : lambda
-        # 'days until easter'                 : lambda
         # 'days since easter'                 : lambda
+        # 'days until easter'                 : lambda
+        # 'easter 2014'                       : lambda
+        # 'fridays in 2015' # rrule
+        # 'fris in 2015' # rrule
+        # 'friday day = 8 in Jan 2015' : lambda r: r == '2015-01-02',
+
+        # '2014 Jan 3:00'                         : lambda r: False,
+        # 'Jan 2014 3:00'                         : lambda r: False,
+        'jan 1 + 99999M'                        : lambda r: r.endswith('01'),
+        '1970 january 1st'                      : lambda r: re.match(YMD_LIST_FORMAT, r), 
+        'day 13 friday in 2021'                 : lambda r: re.match(YMD_LIST_FORMAT, r),
+        'friday day < 13 in 2014 sep'           : lambda r: re.match(YMD_LIST_FORMAT, r),
+        'friday in Jan 2015'                    : lambda r: re.match(YMD_LIST_FORMAT, r),
+        'friday day < 8 in Jan 2015'            : lambda r: r == '2015-01-02',
+        'friday day > 8 in Jan 2015 to Jan 2019': lambda r: re.match(YMD_LIST_FORMAT, r),
+        'friday day < 8 in Jan 2015 to Jan 2019': lambda r: re.match(YMD_LIST_FORMAT, r),
+        'friday day 13 in Jan 2015 to Jan 2019' : lambda r: re.match(YMD_LIST_FORMAT, r),
+        'friday day 13 in August 2021.weekday'  : lambda r: r == 'Friday',
+        'friday day 13 in August 2021'          : lambda r: r == '2021-08-13',
+        'friday day 13 in 2015.weekday'         : lambda r: re.match(DAY_LIST_FORMAT, r),
+        'friday day 13 in 2015'                 : lambda r: re.match(YMD_LIST_FORMAT, r),
+        'fri in 2015'                           : lambda r: re.match(YMD_LIST_FORMAT, r),
+        'friday in 2015'                        : lambda r: re.match(YMD_LIST_FORMAT, r),
+        '2020-01-29 + (1 year + 1 month)'       : lambda r: r == '2021-02-28',
+        'days until Jan 2030'                   : lambda r: float(r) < 3002,
+        'last sun in 2021'                      : lambda r: r == '2021-12-26',
+        'april+1M'                              : lambda r: re.match(YMD_FORMAT, r),
+        't+1d 08h30'                            : lambda r: re.match(ISO_FORMAT, r),
+        '1am t == t 1am'                        : lambda r: eval(r),
+        '1am t'                                 : lambda r: re.match(ISO_FORMAT, r),
+        '(2020-10-10+1d) 3pm'                   : lambda r: '2020-10-11 15:00:00' == r, 
+        't 1:00 == t 1am'                       : lambda r: eval(r),
+        't 1:00'                                : lambda r: re.match(ISO_FORMAT, r),
+        't 1am'                                 : lambda r: re.match(ISO_FORMAT, r),
+        'august'                                : lambda r: re.match(BASEDATE_FORMAT, r),
+        '4th wed in august'                     : lambda r: re.match(YMD_FORMAT, r),
+        '5th sunday in 2021'                    : lambda r: r == '2021-01-31',
+        '4th sunday in 2021'                    : lambda r: r == '2021-01-24',
+        '3rd sunday in 2021'                    : lambda r: r == '2021-01-17',
+        '2nd sunday in 2021'                    : lambda r: r == '2021-01-10',
+        '-1d + 2020-10-10'                      : lambda r: r == '2020-10-09',
+        '2014 Jan + 1M'                         : lambda r: re.match(YMD_FORMAT, r),
+        'Jan 2014 + 1M'                         : lambda r: re.match(YMD_FORMAT, r),
+        'seconds in 24h'                        : lambda r: float(r) == 86400,
+        'today==mon'                            : lambda r: r in ['True', 'False'],
+        'days until mon'                        : lambda r: -4.5 < float(r) < 4.5,
+        'days until next mon'                   : lambda r: 0 <= float(r) <= 7,
+        'next mon + 1d'                         : lambda r: re.match(YMD_FORMAT, r),
+        'monday+1d'                             : lambda r: re.match(YMD_FORMAT, r),
+        'weekday t+100d'                        : lambda r: r in days,
+        '(weekday t+100d)==100d.weekday'        : lambda r: eval(r),
+        '(weekday t+100d)'                      : lambda r: r in days,
+        'weekday tm'                            : lambda r: r in days,
+        'yesterday==thu'                        : lambda r: r in ['True', 'False'],
+        'yesterday==thursday'                   : lambda r: r in ['True', 'False'],
+        'last fri in Dec 2014'                  : lambda r: re.match(YMD_FORMAT, r),
+        'last fri in 2014 Dec'                  : lambda r: re.match(YMD_FORMAT, r),
+        'last fri in 2014 December'             : lambda r: re.match(YMD_FORMAT, r),
+        'days until 2030-12-25'                 : lambda r: float(r) < 3364.55,
+        '6pm+1h'                                : lambda r: re.match(HMS_FORMAT, r),
+        '2014 01'                               : lambda r: re.match(BASEDATE_FORMAT, r), 
+        '1st friday in april'                   : lambda r: re.match(YMD_FORMAT, r) and r.split('-')[1] == '04',
+        'first friday in april'                 : lambda r: re.match(YMD_FORMAT, r) and r.split('-')[1] == '04',
+        '1st friday in next month'              : lambda r: re.match(YMD_FORMAT, r),
+        'first friday in next month'            : lambda r: re.match(YMD_FORMAT, r),
+        'next month'                            : lambda r: re.match(BASEDATE_FORMAT, r),
+        'seconds until 11 pm'                   : lambda r: float(r) < 86400,
+        'seconds until tomorrow'                : lambda r: 0 < float(r) < 86400,
+        '1996 August 28 9 AM'                   : lambda r: r == '1996-08-28 09:00:00',
+        '2s2s'                                  : lambda r: r == '0:00:04',
+        '1 hour in seconds'                     : lambda r: r == '3600.00',
+        '1h in seconds'                         : lambda r: r == '3600.00',
+        '5m+5m'                                 : lambda r: r == '0:10:00',
+        '1957-12-26 22:22:22 in unix'           : lambda r: -379118258 - 86400 < int(r) < -379118258 + 86400,
+        'yd-5h'                                 : lambda r: re.match(ISO_FORMAT, r),
+        '1st sun in April 2021'                 : lambda r: r == '2021-04-04',
+        'first sun in April 2021'               : lambda r: r == '2021-04-04',
+        '1st friday in April 2014'              : lambda r: r == '2014-04-04',
+        'first friday in April 2014'            : lambda r: r == '2014-04-04',
+        'Jan 2014'                              : lambda r: re.match(BASEDATE_FORMAT, r),
+        'weekday 0'                             : lambda r: r in ['Wednesday', 'Thursday'],
+        'wait until (n+.001s)'                  : lambda r: len(r) == 0,
+        'wait .001s'                            : lambda r: len(r) == 0,
+        't - next Sunday'                       : lambda r: re.match(DELTA_FORMAT, r),
+        '2012-12-13-3y.weekday'                 : lambda r: r == 'Sunday',
+        '1st sunday in 2021'                    : lambda r: r == '2021-01-03',
+        'first sunday in 2021'                  : lambda r: r == '2021-01-03',
+        'last sunday in 2021'                   : lambda r: r == '2021-12-26',
+        'last Sunday != next sunday'            : lambda r: r == 'True',
+        'last Sunday == next sunday'            : lambda r: r == 'False',
+        'next Sunday != last sunday'            : lambda r: r == 'True',
+        'next Sunday == last sunday'            : lambda r: r == 'False',
+        'seconds since 3000 Apr 10'             : lambda r: -30899416627.60163 < float(r),
+        'seconds until 3000 Apr 10'             : lambda r: 30899416627.60163 > float(r),
+        '2000-10-10 16:00'                      : lambda r: r == '2000-10-10 16:00:00',
+        '2000-10-10 00:16'                      : lambda r: r == '2000-10-10 00:16:00',
+        'next Sunday'                           : lambda r: re.match(YMD_FORMAT, r),
+        'n'                                     : lambda r: re.match(ISO_FORMAT, r),
+        'YD.day'                                : lambda r: re.match(r'\d+', r),
+        'T.weekday'                             : lambda r: r in days,
+        'T.day'                                 : lambda r: 0 < int(r) < 32,
+        'T-10d'                                 : lambda r: re.match(YMD_FORMAT, r),
+        'T-1.5d'                                : lambda r: re.match(ISO_FORMAT, r),
+        '3M'                                    : lambda r: re.match(DELTA_FORMAT, r),
+        '3h+3M'                                 : lambda r: re.match(DELTA_FORMAT, r),
+        '2h2m'                                  : lambda r: r == '2:02:00',
+        '7y6M5w4d3h2m1.1s'                      : lambda r: re.match(DELTA_FORMAT, r),
+        '1M1d'                                  : lambda r: r == '1 month, 1 day, 0:00:00',
+        '-1y2M'                                 : lambda r: re.match(DELTA_FORMAT, r),
+        '0y2M'                                  : lambda r: r == '2 months',
+        '1y2M'                                  : lambda r: r == '1 year, 2 months',
+        '6y5M4d3h2m1s'                          : lambda r: re.match(DELTA_FORMAT, r),
+        '22h22m'                                : lambda r: r == '22:22:00', 
+        '22h+2m'                                : lambda r: r == '22:02:00', 
+        '12h:00 pm != 12h:00 am'                : lambda r: eval(r),
+        '2 < 1'                                 : lambda r: not eval(r),
+        '2020 Jan 27 + 1y == 2021 Jan 27'       : lambda r: eval(r),
+        '1w'                                    : lambda r: r == '7 days, 0:00:00',
+        '1970 Jan 1 - 3h in unix'               : lambda r: int(r) <= 24*60*60,
+        '1d1m in hours'                         : lambda r: r == '24.02',
+        '1d+0h22m'                              : lambda r: r == '1 day, 0:22:00',
+        '1d'                                    : lambda r: r == '1 day, 0:00:00',
+        '1d in seconds'                         : lambda r: r == '86400.00',
+        '1d in minutes'                         : lambda r: r == '1440.00',
+        '1d in hours'                           : lambda r: r == '24.00',
+        '1958-05-14 - 1958-05-16'               : lambda r: r == '-2 days, 0:00:00',
+        '1957-12-26 22:22:22 - t'               : lambda r: re.match(DELTA_FORMAT, r),
+        '1957-12-26 - t'                        : lambda r: re.match(DELTA_FORMAT, r),
+        '2014 Jan 13==2014 January 13'          : lambda r: eval(r),
+        '12h:00 AM != 12h:00 PM'                : lambda r: eval(r),
+        '1610494238.weekday'                    : lambda r: r == 'Tuesday',
+        '1610494238+4h.weekday'                 : lambda r: r == 'Wednesday',
+        '1610494238'                            : lambda r: '2021-01-12' in r,
+        '1-1-1-1-1-1'                           : lambda r: '0:00:00',
+        '22m:22 + 4h'                           : lambda r: r == '4:22:22',
+        '6pm'                                   : lambda r: re.match(HMS_FORMAT, r),
+        '6 pm + 1h'                             : lambda r: re.match(HMS_FORMAT, r),
+        '6 pm'                                  : lambda r: re.match(HMS_FORMAT, r),
+        '2020-Jan-27'                           : lambda r: r == '2020-01-27',
+        '22:22:22'                              : lambda r: re.match(HMS_FORMAT, r),
+        '22:22:22s'                             : lambda r: r == '22:22:22',
+        '22h:22:22s'                            : lambda r: r == '22:22:22',
+        '22:22m:22s'                            : lambda r: r == '22:22:22',
+        '22h:22m:22s'                           : lambda r: r == '22:22:22',
+        '22h:22m:22'                            : lambda r: r == '22:22:22',
+        '22:22:22'                              : lambda r: r == '22:22:22',
+        '22h:22'                                : lambda r: r == '22:22:00',
+        '1996.04.28'                            : lambda r: r == '1996-04-28',
+        '2014 January 13'                       : lambda r: r == '2014-01-13',
+        '2014 Jan 13'                           : lambda r: r == '2014-01-13',
+        '11:20s PM'                             : lambda r: r == '00:11:20',
+        '11h:20m pm'                            : lambda r: r == '23:20:00',
+        '11h:20 am'                             : lambda r: r == '11:20:00',
+        '11m:20 PM'                             : lambda r: r == '00:11:20',
+        '11h:20 AM'                             : lambda r: r == '11:20:00',
+        '1-1-1 23:23S'                          : lambda r: re.match(ISO_FORMAT, r),
+        '1-1-1 23m:23S'                         : lambda r: re.match(ISO_FORMAT, r),
+        '1-1-1 23m:23s'                         : lambda r: re.match(ISO_FORMAT, r),
+        '1-1-1 23m:23'                          : lambda r: re.match(ISO_FORMAT, r),
+        '1-1-1 23h:23m'                         : lambda r: re.match(ISO_FORMAT, r),
+        '1-1-1 23h:23'                          : lambda r: re.match(ISO_FORMAT, r),
+        '1-1-1 23:23m'                          : lambda r: re.match(ISO_FORMAT, r),
+        '1-1-1 23:23:23'                        : lambda r: re.match(ISO_FORMAT, r),
+        'seconds until 2021 feb 14 12:00:00'    : lambda r: float(r) < 580301.752936,
+        '2021 feb 14 12:00:00'                  : lambda r: r == '2021-02-14 12:00:00',
+        '10h30 + 14h'                           : lambda r: r == '1 day, 0:30:00',
+        'n - 1234'                              : lambda r: re.match(DELTA_FORMAT, r),
+        '1m in hours'                           : lambda r: r == '0.02',
+        '1 in unix'                             : lambda r: r == '1',
+        '08h30'                                 : lambda r: r == '8:30:00',
+        '-1d.weekday'                           : lambda r: r in days,
+        '(t + 180d)-180d == t'                  : lambda r: eval(r),
+        '(n + 181d)-180d != n'                  : lambda r: eval(r),
+        '(n + 180d)-180d == n'                  : lambda r: eval(r),
+        '(T-1d).weekday'                        : lambda r: r in days,
         })
 
 
 def run(test):
     dte_location = os.path.dirname(os.path.realpath(__file__)) \
                              + op.sep + '..' \
                              + (op.sep + 'dte')*2
@@ -215,17 +215,19 @@
 
 
 def make_documentation(test_out):
     import pathlib
     le_path = pathlib.Path(__file__).parent.resolve()
     call(['sed', '-i', '/BEGIN EXAMPLES/q', f'{le_path}/../README.md'])
     with open('../README.md', 'a') as f:
+        f.write('\n|INPUT| OUTPUT |\n')
+        f.write('|-----|--------|\n')
         for test, out in test_out.items():
-            if len(out) < 30:
-                f.write('`' + test + '` returns `' + out + '`\n\n')
+            if '\r' not in out:
+                f.write('|`' + test + '`|`' + out + '`|\n')
 
 
 class Tester(unittest.TestCase):
 
     def test_stuff(self):
         test_out = OrderedDict()
         for test, expectancy in test_expectancy.items():
```

