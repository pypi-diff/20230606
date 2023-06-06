# Comparing `tmp/siat-2.0.8-py3-none-any.whl.zip` & `tmp/siat-2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1135979 bytes, number of entries: 118
+Zip file size: 1136759 bytes, number of entries: 118
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Apr-10 11:29 siat/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-Apr-10 11:29 siat/allin.py
 -rw-rw-rw-  2.0 fat      747 b- defN 23-Apr-10 11:29 siat/alpha_vantage_test.py
 -rw-rw-rw-  2.0 fat    28555 b- defN 23-Apr-10 11:29 siat/assets_liquidity.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-10 11:29 siat/assets_liquidity_test.py
 -rw-rw-rw-  2.0 fat    10110 b- defN 23-Apr-10 11:29 siat/barrons_scraping_test.py
 -rw-rw-rw-  2.0 fat    36597 b- defN 23-Apr-10 11:29 siat/beta_adjustment.py
@@ -86,15 +86,15 @@
 -rw-rw-rw-  2.0 fat    71984 b- defN 23-May-22 08:26 siat/security_prices.py
 -rw-rw-rw-  2.0 fat    10779 b- defN 23-Apr-10 11:29 siat/security_prices_test.py
 -rw-rw-rw-  2.0 fat     1335 b- defN 23-Apr-10 11:29 siat/setup.py
 -rw-rw-rw-  2.0 fat     1418 b- defN 23-Apr-10 11:29 siat/shenwan index history test.py
 -rw-rw-rw-  2.0 fat   118039 b- defN 23-May-26 00:50 siat/stock.py
 -rw-rw-rw-  2.0 fat    31655 b- defN 23-Apr-10 11:29 siat/stock_advice_linear.py
 -rw-rw-rw-  2.0 fat     1312 b- defN 23-Apr-10 11:29 siat/stock_base.py
--rw-rw-rw-  2.0 fat    68123 b- defN 23-Apr-10 11:29 siat/stock_china.py
+-rw-rw-rw-  2.0 fat    72808 b- defN 23-May-28 13:41 siat/stock_china.py
 -rw-rw-rw-  2.0 fat     1276 b- defN 23-Apr-10 11:29 siat/stock_china_test.py
 -rw-rw-rw-  2.0 fat  1242926 b- defN 23-Apr-10 11:29 siat/stock_info.pickle
 -rw-rw-rw-  2.0 fat     6122 b- defN 23-Apr-10 11:29 siat/stock_info_test.py
 -rw-rw-rw-  2.0 fat     1014 b- defN 23-Apr-10 11:29 siat/stock_list_china_test.py
 -rw-rw-rw-  2.0 fat    36738 b- defN 23-Apr-10 11:29 siat/stock_prices_kneighbors.py
 -rw-rw-rw-  2.0 fat    13991 b- defN 23-Apr-10 11:29 siat/stock_prices_linear.py
 -rw-rw-rw-  2.0 fat    25017 b- defN 23-Apr-10 11:29 siat/stock_profile.py
@@ -109,12 +109,12 @@
 -rw-rw-rw-  2.0 fat   118133 b- defN 23-Apr-10 11:29 siat/translate-20230206.py
 -rw-rw-rw-  2.0 fat   121657 b- defN 23-Apr-10 11:29 siat/translate-20230215.py
 -rw-rw-rw-  2.0 fat   126254 b- defN 23-May-25 03:25 siat/translate.py
 -rw-rw-rw-  2.0 fat     3936 b- defN 23-Apr-10 11:29 siat/universal_test.py
 -rw-rw-rw-  2.0 fat    51342 b- defN 23-May-11 00:30 siat/valuation_china.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-10 11:29 siat/valuation_market_china_test.py
 -rw-rw-rw-  2.0 fat    14859 b- defN 23-Apr-10 11:29 siat/var_model_validation.py
--rw-rw-rw-  2.0 fat     1399 b- defN 23-May-27 11:16 siat-2.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 11:16 siat-2.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-27 11:16 siat-2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     9429 b- defN 23-May-27 11:16 siat-2.0.8.dist-info/RECORD
-118 files, 4476991 bytes uncompressed, 1121597 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat     1399 b- defN 23-May-28 13:46 siat-2.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 13:46 siat-2.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-28 13:46 siat-2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     9429 b- defN 23-May-28 13:46 siat-2.0.9.dist-info/RECORD
+118 files, 4481676 bytes uncompressed, 1122377 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -336,20 +336,20 @@
 
 Filename: siat/valuation_market_china_test.py
 Comment: 
 
 Filename: siat/var_model_validation.py
 Comment: 
 
-Filename: siat-2.0.8.dist-info/METADATA
+Filename: siat-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: siat-2.0.8.dist-info/WHEEL
+Filename: siat-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: siat-2.0.8.dist-info/top_level.txt
+Filename: siat-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: siat-2.0.8.dist-info/RECORD
+Filename: siat-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siat/stock_china.py

```diff
@@ -846,32 +846,38 @@
         print(s1)
             
     return
     
 #==============================================================================
 if __name__ =="__main__":
     ticker='000001.SZ'
+    ticker='600519.SS'
     prettytab=True
     tabborder=False
     tabborder=True
 
 def stock_profile_china(ticker,category='profile', \
-                       business_period='recent',financial_quarters=8,valuation_start='2020-1-1', \
-                           prettytab=False,tabborder=False):
+                        business_period='recent', \
+                        financial_quarters=8, \
+                        valuation_start='2020-1-1', \
+                        prettytab=False, \
+                        tabborder=False, \
+                        ):
     """
     功能：介绍中国A股的主要信息，包括公司基本信息、主营信息、股东信息、财务信息、分红历史和市场估值等。
     ticker：A股股票代码
     category：信息类别，默认profile为基本信息，business为主营业务信息，shareholder为股东信息，
     financial为财务基本面，dividend为分红历史，valuation为市场估值信息。
     
-    business_period：介绍主营业务使用的财报期间，默认recent为最近一期（可能为季报、中报或年报），
-    annual为使用最近的年报。
+    business_period：配合category='business'使用，介绍主营业务使用的财报期间，
+    默认recent为最近一期（可能为季报、中报或年报），annual为使用最近的年报。
+    
+    financial_quarters：配合category='financial'使用，介绍财务基本面使用的季度个数，最大为8.
+    valuation_start：配合category='valuation'使用，介绍市场估值信息时使用的开始日期，默认为2020-1-1。
     
-    financial_quarters：介绍财务基本面使用的季度个数，最大为8.
-    valuation_start：介绍市场估值信息时使用的开始日期，默认为2020-1-1。
     prettytab：输出表格样式，默认False使用markdown报表，True使用prettytable报表
     tabborder：prettytable报表时是否绘制边框，默认不绘制False，True绘制简单字符链接的边框，丑陋。
     
     返回值：无。
     建议运行环境：Anaconda Jupyter Notebook，其他环境未测试。
     """
     
@@ -993,34 +999,55 @@
         print_sentence(longtext,mid_symbol=['；','。'])
             
         print("\n*** 机构简介：")
         longtext=df6.iloc[0]["机构简介"]
         print_sentence(longtext,mid_symbol=['；','。'])
 
     # 主营业务信息查询=============================================================================
+    # 主营业务仅在年报/中报中公布，一三季报中无此信息
     if category == 'business':
         try:
             df2=ak.stock_zygc_ym(symbol=ticker1)  
         except:
             print("  #Warning(stock_profile_china): business info not found for",ticker)
             return
         
         df2['分类']=df2['分类'].apply(lambda x: '***合计' if x=='合计' else x)
     
         # 整理信息
-        if business_period == 'annual':    #最近一期年报
-            df2['报告类别']=df2['报告期'].apply(lambda x: x[-2:])
-            df2a=df2[df2['报告类别']=='年度'].copy(deep=True)
-            df2a.reset_index(drop=True,inplace=True)
+        df2['报告年度']=df2['报告期'].apply(lambda x: x[:4])
+        df2['报告类别']=df2['报告期'].apply(lambda x: x[-2:])
+        df2['报告月日']=df2['报告类别'].apply(lambda x: '12-31' if x=='年度' else '06-30' if x=='中期' else '12-31')
+        df2['报告日期']=df2['报告年度']+'-'+df2['报告月日']
+        
+        if business_period in ['annual','recent']:
+            if business_period == 'annual':    #最近一期年报
+                df2a=df2[df2['报告类别']=='年度'].copy(deep=True)
+                df2a.reset_index(drop=True,inplace=True)
+            if business_period == 'recent':    #最近一期年报/中报
+                df2a=df2.copy(deep=True)
+
             period=df2a.head(1)['报告期'][0]
-            del df2['报告类别']
-        else:   #最近一期财报，可能是季报、中报或年报
-            period=df2.head(1)['报告期'][0]
+        else:   #具体中报或年报日期
+            result,business_period1=check_date2(business_period)
+            if result:
+                df2a=df2[df2['报告日期']==business_period1].copy(deep=True)
+                if len(df2a) > 0:
+                    df2a.reset_index(drop=True,inplace=True)
+                    period=df2a.head(1)['报告期'][0]
+                else:
+                    print("  #Warning(stock_profile_china): invalid business period for",business_period)
+                    print("  Valid business_period: annual, recent, or an valid mid-term/annual report date, eg 2022-12-31 or 2022-6-30")
+                    return
+            else:
+                print("  #Warning(stock_profile_china): invalid business period for",business_period)
+                print("  Valid business_period: annual, recent, or an valid mid-term/annual report date, eg 2022-12-31 or 2022-6-30")
+                return
+            
         dftmp=df2[df2['报告期']==period]
-        del dftmp['报告期']
         
         cols1=['分类方向','分类','营业收入','营业收入-占主营收入比','营业成本','营业成本-占主营成本比','毛利率']
         cols2=['分类方向','分类','营业收入-同比增长','营业成本-同比增长','毛利率','毛利率-同比增长']
         
         dftmp1=dftmp[cols1]        
         titletxt1=codetranslate(ticker)+'：主营业务构成，'+period+'财报'
         if prettytab:
@@ -1042,14 +1069,23 @@
             print('\n数据来源：益盟-F10,',str(today))
 
     # 历史分红信息查询=============================================================================
     if category == 'dividend':
         try:
             df3=ak.stock_dividents_cninfo(symbol=ticker1)  
         except:
+            try:
+                # 测试是否akshare本身出现问题
+                tmpdf3=ak.stock_dividents_cninfo(symbol='600519')
+            except:
+                # akshare本身出现问题
+                print("  #Warning(stock_profile_china): problem incurred for akshare")
+                print("  Try upgrade akshare using: pip install akshare --upgrade")
+                print("  If same problem remains, try upgrade akshare again later")
+                return
             print("  #Warning(stock_profile_china): dividend info not found for",ticker)
             return
     
         # 整理信息
         df3.fillna('',inplace=True)
         dftmp=df3.copy(deep=True)
         dftmp.drop(['实施方案公告日期','股份到账日'],axis=1,inplace=True)
@@ -1060,15 +1096,15 @@
         newcols=['报告时间','送股比例','转增比例','派息比例','股权登记日','除权日','派息日','实施方案分红说明']
         dftmp1=dftmp[newcols]
         
         # 替换送转派息字段中的零为空，全局替换
         dftmp2=dftmp1.replace(0,'')
         dftmp3=dftmp2.replace('','--')
 
-        titletxt=codetranslate(ticker)+'：分红历史'
+        titletxt=codetranslate(ticker)+'：股利发放历史'
         if prettytab:
             pandas2prettytable(dftmp3,titletxt,firstColSpecial=False,leftColAlign='l',otherColAlign='c',tabborder=tabborder)
             print(' ','数据来源：巨潮资讯,',str(today))
         else:
             print('\n*** '+titletxt+'\n')
             print(dftmp3.to_markdown(tablefmt='Simple',index=False,colalign=['left','center','center','right','center','center','center','left']))
             print('\n数据来源：巨潮资讯,',str(today))
@@ -1079,27 +1115,71 @@
         try:
             df4=ak.stock_main_stock_holder(stock=ticker1)  
         except:
             print("  #Warning(stock_profile_china): shareholder info not found for",ticker)
             return
     
         # 整理信息
-        df4.fillna('',inplace=True)
-        dftmp=df4.head(10).copy(deep=True)
-        enddate=dftmp.head(1)['截至日期'][0]
+        #df4.fillna('',inplace=True)
+        df4.fillna(0,inplace=True)
+        
+        #df4['报告年度']=df4['截至日期'].apply(lambda x: x.year)
+        df4['报告年度']=df4['截至日期'].apply(lambda x: x.strftime("%Y"))
+        df4['报告月日']=df4['截至日期'].apply(lambda x: x.strftime("%m-%d"))
+        df4['报告类别']=df4['报告月日'].apply(lambda x: '年度' if x=='12-31' else '中期' if x=='06-30' else '季度')
+        
+        if business_period in ['annual','recent']:
+            if business_period == 'annual':    #最近一期年报
+                df4a=df4[df4['报告类别']=='年度'].copy(deep=True)
+                df4a.reset_index(drop=True,inplace=True)
+            if business_period == 'recent':    #最近一期年报/中报
+                df4a=df4.copy(deep=True)
+
+            period=df4a.head(1)['截至日期'][0]
+        else:   #具体财报日期
+            result,business_period1=check_date2(business_period)
+            if result:
+                # 转换为字符串类型，否则比较失败
+                df4['截至日期1']=df4['截至日期'].apply(lambda x:str(x))
+                df4a=df4[df4['截至日期1']==business_period1].copy(deep=True)
+                if len(df4a) > 0:
+                    df4a.reset_index(drop=True,inplace=True)
+                    period=df4a.head(1)['截至日期'][0]
+                else:
+                    print("  #Warning(stock_profile_china): invalid business period for",business_period)
+                    print("  Valid business_period: annual, recent, or an valid mid-term/annual report date, eg 2022-12-31")
+                    return
+            else:
+                print("  #Warning(stock_profile_china): invalid business period for",business_period)
+                print("  Valid business_period: annual, recent, or an valid mid-term/annual report date, eg 2022-6-30")
+                return
+            
+        dftmp=df4a.head(10).copy(deep=True)
+        
+        enddate=str(dftmp.head(1)['截至日期'][0])
         shareholder_num=dftmp.head(1)['股东总数'][0]
         avg_shares=dftmp.head(1)['平均持股数'][0]
-        titletxt=codetranslate(ticker)+'：十大股东（截至'+enddate+'，股东总数'+shareholder_num+'，平均持股数'+avg_shares+'）'
+        titletxt=codetranslate(ticker)+'：十大股东（截至'+str(enddate)+'，股东总数'+str(int(shareholder_num))+'，平均持股数'+str(int(avg_shares))+'）'
         
         dftmp.drop(['截至日期','公告日期','股东说明','股东总数','平均持股数'],axis=1,inplace=True)
         
-        dftmp['持股数量(股)']=dftmp['持股数量(股)'].apply(lambda x: mstring2number(x))
-        dftmp['持股数量(百万股)']=dftmp['持股数量(股)'].apply(lambda x: round(x / baiwan,2))
-        
-        dftmp['持股比例(%)']=dftmp['持股比例(%)'].apply(lambda x: mstring2number(x,'float'))
+        #dftmp['持股数量(股)']=dftmp['持股数量(股)'].apply(lambda x: mstring2number(x))
+        #dftmp['持股数量']=dftmp['持股数量'].apply(lambda x: mstring2number(x))
+        dftmp['持股数量']=dftmp['持股数量'].apply(lambda x: float(x))
+        #dftmp['持股数量(百万股)']=dftmp['持股数量(股)'].apply(lambda x: round(x / baiwan,2))
+        dftmp['持股数量(百万股)']=dftmp['持股数量'].apply(lambda x: round(x / baiwan,2))
+        
+        #dftmp['持股比例(%)']=dftmp['持股比例'].apply(lambda x: mstring2number(x,'float'))
+        dftmp['持股比例(%)']=dftmp['持股比例']
+        
+        # 检查持股比例是否异常
+        check_holding=dftmp.head(1)['持股比例'][0]
+        if check_holding ==0.0:
+            print("  #Warning(stock_profile_china): shareholder holding info seems weired")
+            dftmp=dftmp.replace(0,'---')
         
         newcols=['编号','股东名称','股本性质','持股比例(%)','持股数量(百万股)']
         dftmp1=dftmp[newcols]        
         
         if prettytab:
             pandas2prettytable(dftmp1,titletxt,firstColSpecial=False,leftColAlign='c',otherColAlign='c',tabborder=tabborder)
             print(' ','数据来源：新浪财经,',str(today))
@@ -1108,15 +1188,16 @@
             print(dftmp1.to_markdown(tablefmt='Simple',index=False,colalign=['center','left','left','right','right']))
             print('\n数据来源：新浪财经,',str(today))
 
 
     # 主要市场指标查询=============================================================================
     if category == 'valuation':
         try:
-            df5=ak.stock_a_lg_indicator(symbol=ticker1)  
+            #df5=ak.stock_a_lg_indicator(symbol=ticker1)  
+            df5=ak.stock_a_indicator_lg(symbol=ticker1)  
         except:
             print("  #Warning(stock_profile_china): valuation spyder failed or info not found for",ticker)
             return
     
         # 整理信息
         import pandas as pd
         start=valuation_start
```

## Comparing `siat-2.0.8.dist-info/METADATA` & `siat-2.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siat
-Version: 2.0.8
+Version: 2.0.9
 Summary: Securities Investment Analysis Tools (siat)
 Home-page: https://pypi.org/project/siat/
 Author: Prof. WANG Dehong, Business School, BFSU (北京外国语大学 国际商学院 王德宏 教授)
 Author-email: wdehong2000@163.com
 License: Copyright (C) WANG Dehong, 2023. For educational purpose only!
 Platform: UNKNOWN
 Requires-Dist: pandas-datareader
```

## Comparing `siat-2.0.8.dist-info/RECORD` & `siat-2.0.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 siat/security_prices.py,sha256=vmN39llWbm-B1awfuZzR14UlEca6Tm3KOvBQUYZJzXw,71984
 siat/security_prices_test.py,sha256=OEphoJ87NPKoNow1QA8EU_5MUYrJF-qKoWKNapVfZNI,10779
 siat/setup.py,sha256=up65rQGLmTBkhtaMLowjoQXYmIsnycnm4g1SYmeQS6o,1335
 siat/shenwan index history test.py,sha256=JCVAzOSEldHalhSFa3pqD8JI_8_djPMQOxpkuYU-Esg,1418
 siat/stock.py,sha256=unwmbNTT5vC3v9cg4XtnpPBawPVxtBTgRnevE1i0T00,118039
 siat/stock_advice_linear.py,sha256=-twT7IGP-NEplkL1WPSACcNJjggRB2j4mlAQCkzOAuo,31655
 siat/stock_base.py,sha256=uISvbRyOGy8p9QREA96CVydgflBkn5L3OXOGKl8oanc,1312
-siat/stock_china.py,sha256=qsrGq5tUyToOGDfVRnMEeiGps2Tpz5o38LlK6kB6k3Y,68123
+siat/stock_china.py,sha256=ELE3Agl6eUvA8_Gec6EkxbCvQ53OWzlmy067-hj6Bdo,72808
 siat/stock_china_test.py,sha256=Qc1m19FAUSvBi9E0ZTVcYBveiGYFIlIFvthbidzCe1s,1276
 siat/stock_info.pickle,sha256=gzhzPvCrX3tr24CzWPVAOXPJ21XQ5keU2cz6PfKwfJ8,1242926
 siat/stock_info_test.py,sha256=gfG3DbhDACbtD8wnv_R6zhj0t11XaC8NX8uLD9Qv3Fo,6122
 siat/stock_list_china_test.py,sha256=gv14UwMMvkZqtb6G7DCTSuehIwVHuVwu7w60p6gyHoo,1014
 siat/stock_prices_kneighbors.py,sha256=WfZvo5EyeBsm-T37zDj7Sl9dPSRq5Bx4JxIJ9IUum6s,36738
 siat/stock_prices_linear.py,sha256=-OUKRr27L2aStQgJSlJOrJ4gay_G7P-m-7t7cU2Yoqk,13991
 siat/stock_profile.py,sha256=kEoYOsHm0Kc75gEVchDbPbJNfzPvNi6QKTxMySo_2Fg,25017
@@ -108,11 +108,11 @@
 siat/translate-20230206.py,sha256=-vtI125WyaJhmPotOpDAmclt_XnYVaWU9ByLWZ6FyYE,118133
 siat/translate-20230215.py,sha256=TJgtPE3n8IjljmZ4Pefy8dmHoNdFF-1zpML6BhA9FKE,121657
 siat/translate.py,sha256=pW6jWGfuypUNgZiu_ojJLsaEOEb12XWDzdp77z1sG3I,126254
 siat/universal_test.py,sha256=CDAOffW1Rvs-TcNN5giWVvHMlch1w4dp-w5SIV9jXL0,3936
 siat/valuation_china.py,sha256=gYYXeT9bBPyQ251TCsYlibWcu6JA8x-YOKqLUEeLE7U,51342
 siat/valuation_market_china_test.py,sha256=gbJ0ioauuo4koTPH6WKUkqcXiQPafnbhU5eKJ6lpdLA,1571
 siat/var_model_validation.py,sha256=zB_Skk_tmzIR15l6oAW3am4HBGVIG-eZ8gJhCdXZ8Qw,14859
-siat-2.0.8.dist-info/METADATA,sha256=mDOyGH3sWynimC6vhxnpiD4daBL_EvEwnMsEFVFWw2g,1399
-siat-2.0.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-siat-2.0.8.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
-siat-2.0.8.dist-info/RECORD,,
+siat-2.0.9.dist-info/METADATA,sha256=o3R7xY-l_dmZxa2V26ztqkWmMDGG3Lr5_oJ3WbYsal8,1399
+siat-2.0.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+siat-2.0.9.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
+siat-2.0.9.dist-info/RECORD,,
```

