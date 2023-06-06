# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.906.tar", last modified: Mon Jun  5 00:27:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.907.tar", last modified: Tue Jun  6 02:19:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.906.tar` & `tencentcloud-sdk-python-billing-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)     2904 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155292 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)    20134 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:27:15.000000 tencentcloud-sdk-python-billing-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   166860 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)    21124 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:19:20.000000 tencentcloud-sdk-python-billing-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-billing-3.0.906/README.rst` & `tencentcloud-sdk-python-billing-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.907/tencentcloud/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.906'
+__version__ = '3.0.907'
```

### Comparing `tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -649,14 +649,68 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BusinessSummaryInfo(AbstractModel):
+    """产品汇总信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BusinessCode: 产品编码
+        :type BusinessCode: str
+        :param BusinessCodeName: 产品名称：用户所采购的各类云产品，例如：云服务器 CVM
+        :type BusinessCodeName: str
+        :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCost: str
+        :param RealTotalCost: 优惠后总价
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
+        :type CashPayAmount: str
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
+        :type IncentivePayAmount: str
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
+        :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
+        """
+        self.BusinessCode = None
+        self.BusinessCodeName = None
+        self.TotalCost = None
+        self.RealTotalCost = None
+        self.CashPayAmount = None
+        self.IncentivePayAmount = None
+        self.VoucherPayAmount = None
+        self.TransferPayAmount = None
+
+
+    def _deserialize(self, params):
+        self.BusinessCode = params.get("BusinessCode")
+        self.BusinessCodeName = params.get("BusinessCodeName")
+        self.TotalCost = params.get("TotalCost")
+        self.RealTotalCost = params.get("RealTotalCost")
+        self.CashPayAmount = params.get("CashPayAmount")
+        self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BusinessSummaryOverviewItem(AbstractModel):
     """按产品汇总产品详情
 
     """
 
     def __init__(self):
         r"""
@@ -978,28 +1032,48 @@
         :type BusinessCode: str
         :param BusinessCodeName: 产品名称
         :type BusinessCodeName: str
         :param RealTotalCost: 折后总价
         :type RealTotalCost: str
         :param Trend: 费用趋势
         :type Trend: :class:`tencentcloud.billing.v20180709.models.ConsumptionSummaryTrend`
+        :param CashPayAmount: 现金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CashPayAmount: str
+        :param IncentivePayAmount: 赠送金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IncentivePayAmount: str
+        :param VoucherPayAmount: 代金券
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
         """
         self.BusinessCode = None
         self.BusinessCodeName = None
         self.RealTotalCost = None
         self.Trend = None
+        self.CashPayAmount = None
+        self.IncentivePayAmount = None
+        self.VoucherPayAmount = None
+        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.BusinessCode = params.get("BusinessCode")
         self.BusinessCodeName = params.get("BusinessCodeName")
         self.RealTotalCost = params.get("RealTotalCost")
         if params.get("Trend") is not None:
             self.Trend = ConsumptionSummaryTrend()
             self.Trend._deserialize(params.get("Trend"))
+        self.CashPayAmount = params.get("CashPayAmount")
+        self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1018,20 +1092,36 @@
         :type ProjectName: str
         :param RealTotalCost: 折后总价
         :type RealTotalCost: str
         :param Trend: 趋势
         :type Trend: :class:`tencentcloud.billing.v20180709.models.ConsumptionSummaryTrend`
         :param Business: 产品消耗详情
         :type Business: list of ConsumptionBusinessSummaryDataItem
+        :param CashPayAmount: 现金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CashPayAmount: str
+        :param IncentivePayAmount: 赠送金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IncentivePayAmount: str
+        :param VoucherPayAmount: 代金券
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
         """
         self.ProjectId = None
         self.ProjectName = None
         self.RealTotalCost = None
         self.Trend = None
         self.Business = None
+        self.CashPayAmount = None
+        self.IncentivePayAmount = None
+        self.VoucherPayAmount = None
+        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.ProjectId = params.get("ProjectId")
         self.ProjectName = params.get("ProjectName")
         self.RealTotalCost = params.get("RealTotalCost")
         if params.get("Trend") is not None:
@@ -1039,14 +1129,18 @@
             self.Trend._deserialize(params.get("Trend"))
         if params.get("Business") is not None:
             self.Business = []
             for item in params.get("Business"):
                 obj = ConsumptionBusinessSummaryDataItem()
                 obj._deserialize(item)
                 self.Business.append(obj)
+        self.CashPayAmount = params.get("CashPayAmount")
+        self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1184,28 +1278,64 @@
         :type PayModeName: str
         :param BusinessCode: 产品名称代码
         :type BusinessCode: str
         :param BusinessCodeName: 产品名称
         :type BusinessCodeName: str
         :param ConsumptionTypeName: 消耗类型
         :type ConsumptionTypeName: str
+        :param RealCost: 折前价
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RealCost: str
+        :param FeeBeginTime: 费用起始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FeeBeginTime: str
+        :param FeeEndTime: 费用结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FeeEndTime: str
+        :param DayDiff: 天数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DayDiff: str
+        :param DailyTotalCost: 每日消耗
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DailyTotalCost: str
+        :param OrderId: 订单号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OrderId: str
+        :param VoucherPayAmount: 代金券
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VoucherPayAmount: str
+        :param IncentivePayAmount: 赠送金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IncentivePayAmount: str
+        :param TransferPayAmount: 分成金
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
         """
         self.ResourceId = None
         self.ResourceName = None
         self.RealTotalCost = None
         self.CashPayAmount = None
         self.ProjectId = None
         self.ProjectName = None
         self.RegionId = None
         self.RegionName = None
         self.PayMode = None
         self.PayModeName = None
         self.BusinessCode = None
         self.BusinessCodeName = None
         self.ConsumptionTypeName = None
+        self.RealCost = None
+        self.FeeBeginTime = None
+        self.FeeEndTime = None
+        self.DayDiff = None
+        self.DailyTotalCost = None
+        self.OrderId = None
+        self.VoucherPayAmount = None
+        self.IncentivePayAmount = None
+        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.ResourceId = params.get("ResourceId")
         self.ResourceName = params.get("ResourceName")
         self.RealTotalCost = params.get("RealTotalCost")
         self.CashPayAmount = params.get("CashPayAmount")
@@ -1214,14 +1344,23 @@
         self.RegionId = params.get("RegionId")
         self.RegionName = params.get("RegionName")
         self.PayMode = params.get("PayMode")
         self.PayModeName = params.get("PayModeName")
         self.BusinessCode = params.get("BusinessCode")
         self.BusinessCodeName = params.get("BusinessCodeName")
         self.ConsumptionTypeName = params.get("ConsumptionTypeName")
+        self.RealCost = params.get("RealCost")
+        self.FeeBeginTime = params.get("FeeBeginTime")
+        self.FeeEndTime = params.get("FeeEndTime")
+        self.DayDiff = params.get("DayDiff")
+        self.DailyTotalCost = params.get("DailyTotalCost")
+        self.OrderId = params.get("OrderId")
+        self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2454,14 +2593,76 @@
                 self.SummaryOverview.append(obj)
         if params.get("SummaryTotal") is not None:
             self.SummaryTotal = SummaryTotal()
             self.SummaryTotal._deserialize(params.get("SummaryTotal"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeBillSummaryRequest(AbstractModel):
+    """DescribeBillSummary请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Month: 账单月份，格式为2023-04
+        :type Month: str
+        :param GroupType: 账单维度类型，枚举值如下：business、project、region、payMode、tag
+        :type GroupType: str
+        :param TagKey: 标签键，GroupType=tag获取标签维度账单时传
+        :type TagKey: list of str
+        """
+        self.Month = None
+        self.GroupType = None
+        self.TagKey = None
+
+
+    def _deserialize(self, params):
+        self.Month = params.get("Month")
+        self.GroupType = params.get("GroupType")
+        self.TagKey = params.get("TagKey")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeBillSummaryResponse(AbstractModel):
+    """DescribeBillSummary返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Ready: 数据是否准备好，0准备中，1已就绪。（Ready=0，为当前UIN首次进行初始化出账，预计需要5~10分钟出账，请于10分钟后重试即可）
+        :type Ready: int
+        :param SummaryDetail: 账单多维度汇总消费详情
+        :type SummaryDetail: list of SummaryDetail
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Ready = None
+        self.SummaryDetail = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Ready = params.get("Ready")
+        if params.get("SummaryDetail") is not None:
+            self.SummaryDetail = []
+            for item in params.get("SummaryDetail"):
+                obj = SummaryDetail()
+                obj._deserialize(item)
+                self.SummaryDetail.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeCostDetailRequest(AbstractModel):
     """DescribeCostDetail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2554,17 +2755,17 @@
 
     def __init__(self):
         r"""
         :param BeginTime: 目前必须和EndTime相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type BeginTime: str
         :param EndTime: 目前必须和BeginTime为相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type EndTime: str
-        :param Limit: 每次获取数据量
+        :param Limit: 每次获取数据量，最大值为100
         :type Limit: int
-        :param Offset: 偏移量
+        :param Offset: 偏移量,默认从0开始
         :type Offset: int
         :param PayerUin: 查询账单数据的用户UIN
         :type PayerUin: str
         :param NeedRecordNum: 是否需要返回记录数量，0不需要，1需要，默认不需要
         :type NeedRecordNum: int
         """
         self.BeginTime = None
@@ -2640,17 +2841,17 @@
 
     def __init__(self):
         r"""
         :param BeginTime: 目前必须和EndTime相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type BeginTime: str
         :param EndTime: 目前必须和BeginTime为相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type EndTime: str
-        :param Limit: 每次获取数据量
+        :param Limit: 每次获取数据量，最大值为100
         :type Limit: int
-        :param Offset: 偏移量
+        :param Offset: 偏移量,默认从0开始
         :type Offset: int
         :param PayerUin: 查询账单数据的用户UIN
         :type PayerUin: str
         :param NeedRecordNum: 是否需要返回记录数量，0不需要，1需要，默认不需要
         :type NeedRecordNum: int
         """
         self.BeginTime = None
@@ -2724,17 +2925,17 @@
 
     def __init__(self):
         r"""
         :param BeginTime: 目前必须和EndTime相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type BeginTime: str
         :param EndTime: 目前必须和BeginTime为相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type EndTime: str
-        :param Limit: 每次获取数据量
+        :param Limit: 每次获取数据量，最大值为100
         :type Limit: int
-        :param Offset: 偏移量
+        :param Offset: 偏移量,默认从0开始
         :type Offset: int
         :param PayerUin: 查询账单数据的用户UIN
         :type PayerUin: str
         :param NeedRecordNum: 是否需要返回记录数量，0不需要，1需要，默认不需要
         :type NeedRecordNum: int
         """
         self.BeginTime = None
@@ -2809,17 +3010,17 @@
 
     def __init__(self):
         r"""
         :param BeginTime: 目前必须和EndTime相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type BeginTime: str
         :param EndTime: 目前必须和BeginTime为相同月份，不支持跨月查询，且查询结果是整月数据，例如 BeginTime为2018-09，EndTime 为 2018-09，查询结果是 2018 年 9 月数据。
         :type EndTime: str
-        :param Limit: 每次获取数据量
+        :param Limit: 每次获取数据量，最大值为100
         :type Limit: int
-        :param Offset: 偏移量
+        :param Offset: 偏移量,默认从0开始
         :type Offset: int
         :param PayerUin: 查询账单数据的用户UIN
         :type PayerUin: str
         :param NeedRecordNum: 是否需要返回记录数量，0不需要，1需要，默认不需要
         :type NeedRecordNum: int
         :param NeedConditionValue: 是否需要返回过滤条件，0不需要，1需要，默认不需要
         :type NeedConditionValue: int
@@ -3712,14 +3913,79 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SummaryDetail(AbstractModel):
+    """账单多维度汇总消费详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GroupKey: 账单维度编码
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GroupKey: str
+        :param GroupValue: 账单维度值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GroupValue: str
+        :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
+        :type TotalCost: str
+        :param RealTotalCost: 优惠后总价
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
+        :type CashPayAmount: str
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
+        :type IncentivePayAmount: str
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
+        :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
+        :param Business: 产品汇总信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Business: list of BusinessSummaryInfo
+        """
+        self.GroupKey = None
+        self.GroupValue = None
+        self.TotalCost = None
+        self.RealTotalCost = None
+        self.CashPayAmount = None
+        self.IncentivePayAmount = None
+        self.VoucherPayAmount = None
+        self.TransferPayAmount = None
+        self.Business = None
+
+
+    def _deserialize(self, params):
+        self.GroupKey = params.get("GroupKey")
+        self.GroupValue = params.get("GroupValue")
+        self.TotalCost = params.get("TotalCost")
+        self.RealTotalCost = params.get("RealTotalCost")
+        self.CashPayAmount = params.get("CashPayAmount")
+        self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
+        if params.get("Business") is not None:
+            self.Business = []
+            for item in params.get("Business"):
+                obj = BusinessSummaryInfo()
+                obj._deserialize(item)
+                self.Business.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class SummaryTotal(AbstractModel):
     """总数
 
     """
```

### Comparing `tencentcloud-sdk-python-billing-3.0.906/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.907/tencentcloud/billing/v20180709/billing_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeBillSummary(self, request):
+        """该接口支持通过传参，按照产品、项目、地域、计费模式和标签五个维度获取账单费用明细。
+
+        :param request: Request instance for DescribeBillSummary.
+        :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryRequest`
+        :rtype: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBillSummary", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBillSummaryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeBillSummaryByPayMode(self, request):
         """获取按计费模式汇总费用分布
 
         :param request: Request instance for DescribeBillSummaryByPayMode.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByPayModeRequest`
         :rtype: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByPayModeResponse`
```

### Comparing `tencentcloud-sdk-python-billing-3.0.906/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.907/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.907/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.906/setup.py` & `tencentcloud-sdk-python-billing-3.0.907/setup.py`

 * *Files identical despite different names*

