# Comparing `tmp/finqual-1.0.0.tar.gz` & `tmp/finqual-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finqual-1.0.0.tar", last modified: Sun Jul 16 22:47:18 2023, max compression
+gzip compressed data, was "finqual-1.1.0.tar", last modified: Tue Jul 18 22:37:37 2023, max compression
```

## Comparing `finqual-1.0.0.tar` & `finqual-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.369020 finqual-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4874 2023-07-16 22:47:18.369020 finqual-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4352 2023-07-16 22:41:03.000000 finqual-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.364015 finqual-1.0.0/finqual/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-1.0.0/finqual/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.368019 finqual-1.0.0/finqual/data/
--rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-1.0.0/finqual/data/sec_sic.csv
--rw-rw-rw-   0        0        0   130768 2023-07-15 09:40:35.000000 finqual-1.0.0/finqual/finqual.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:47:18.367017 finqual-1.0.0/finqual.egg-info/
--rw-rw-rw-   0        0        0     4874 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 22:47:18.000000 finqual-1.0.0/finqual.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 22:47:18.369020 finqual-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-07-16 22:46:45.000000 finqual-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:37:37.139372 finqual-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-07-17 21:30:26.000000 finqual-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4929 2023-07-18 22:37:37.139372 finqual-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4409 2023-07-18 22:33:40.000000 finqual-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 22:37:37.127484 finqual-1.1.0/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-1.1.0/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:37:37.137371 finqual-1.1.0/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-1.1.0/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   136015 2023-07-18 22:03:09.000000 finqual-1.1.0/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:37:37.133366 finqual-1.1.0/finqual.egg-info/
+-rw-rw-rw-   0        0        0     4929 2023-07-18 22:37:37.000000 finqual-1.1.0/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-18 22:37:37.000000 finqual-1.1.0/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 22:37:37.000000 finqual-1.1.0/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 22:37:37.000000 finqual-1.1.0/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 22:37:37.139372 finqual-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      830 2023-07-18 22:35:51.000000 finqual-1.1.0/setup.py
```

### Comparing `finqual-1.0.0/LICENSE.txt` & `finqual-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-1.0.0/PKG-INFO` & `finqual-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
-Author: Myztika
+Author: Harry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -79,21 +79,21 @@
 
 The `ratios` function calculates selected financial ratios for the specified timeframe and returns the mean average over that timeframe. The selected financial ratios are a selection of liquidity, profitability and valuation ratios, which are commonly used to compare against other companies,
 
 The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible within the package.
 
 ## Dependencies
 
-Only four packages are required, with the following versions confirmed to be working:
+Only five packages are required, with the following versions confirmed to be working:
 
 | Package   | Version   |
 |-----------|-----------|
 | pandas    | >= 2.0.2  |
 | numpy     | >= 1.24.3 |
 | requests  | >= 2.28.1 |
 | ratelimit | >= 2.2.1  |
 | datetime  | >= 5.1    |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
-- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database
+- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database or use the IFRS taxonomy instead of the US GAAP taxonomy
```

### Comparing `finqual-1.0.0/README.md` & `finqual-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,21 @@
 
 The `ratios` function calculates selected financial ratios for the specified timeframe and returns the mean average over that timeframe. The selected financial ratios are a selection of liquidity, profitability and valuation ratios, which are commonly used to compare against other companies,
 
 The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible within the package.
 
 ## Dependencies
 
-Only four packages are required, with the following versions confirmed to be working:
+Only five packages are required, with the following versions confirmed to be working:
 
 | Package   | Version   |
 |-----------|-----------|
 | pandas    | >= 2.0.2  |
 | numpy     | >= 1.24.3 |
 | requests  | >= 2.28.1 |
 | ratelimit | >= 2.2.1  |
 | datetime  | >= 5.1    |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
-- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database
+- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database or use the IFRS taxonomy instead of the US GAAP taxonomy
```

### Comparing `finqual-1.0.0/finqual/data/sec_sic.csv` & `finqual-1.1.0/finqual/data/sec_sic.csv`

 * *Files identical despite different names*

### Comparing `finqual-1.0.0/finqual/finqual.py` & `finqual-1.1.0/finqual/finqual.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,31 +177,33 @@
 
         url = 'https://data.sec.gov/api/xbrl/companyfacts/CIK' + value + '.json'
 
         # Getting the Pandas dataframe of chosen ticker
         source = requests.get(url=url, headers=headers, verify=True)
         data = source.json()
         data = pd.DataFrame(data)
-
-        return data["facts"]
+        try:
+            return data["facts"]["ifrs-full"]
+        except:
+            return data["facts"]["us-gaap"]
 
     def lookup(self, node, year, category, quarter = None):
         """
         Looks up items that are under the "us-gaap" taxonomy and are in USD units, this has to be done year by year or quarter
         by quarter as companies may change what they file certain items under
         """
         item = node.name
         data = self.data
 
         if (category == "income"):
             """
             Creating search term
             """
             try:
-                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD"])
+                df = pd.DataFrame(pd.DataFrame(data[item])["units"][0])
                 df.dropna(inplace = True)
                 df["frame"] = df["frame"].str.replace('I', '')
 
                 if (quarter != None):
                     # If looking at quarter then:
                     search = "CY" + str(year) + "Q" + str(quarter)
                 else:
@@ -209,15 +211,15 @@
 
                 return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
 
             except:
                 pass
 
             try:
-                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD/shares"])
+                df = pd.DataFrame(pd.DataFrame(data[item])["units"][0])
                 df.dropna(inplace=True)
                 df["frame"] = df["frame"].str.replace('I', '')
 
                 if (quarter != None):
                     # If looking at quarter then:
                     search = "CY" + str(year) + "Q" + str(quarter)
                 else:
@@ -231,15 +233,15 @@
         if (category == "balance"):
 
             """
             Getting the desired item value
             """
             try:
 
-                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD"])
+                df = pd.DataFrame(pd.DataFrame(data[item])["units"][0])
                 df.dropna(inplace = True)
                 df["frame"] = df["frame"].str.replace('I', '')
                 fy = df[df["fp"] == "FY"].iloc[-1][7][-2:]
 
                 if (quarter == None):
                     search = "CY" + str(year) + fy
                 else:
@@ -249,15 +251,15 @@
 
             except:
 
                 return False
 
         if (category == "cashflow"):
             try:
-                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD"])
+                df = pd.DataFrame(pd.DataFrame(data[item])["units"][0])
             except:
                 return False
 
             if (df.shape[1] == 8):
                 try:
                     df.drop_duplicates(subset=["end", "val"], inplace=True, keep="last")
                     df['end'] = pd.to_datetime(df["end"], format='%Y-%m-%d')
@@ -376,16 +378,16 @@
         year_list = [i for i in np.arange(end, start - 2, -1)]
         quarter_list = [str(i) + "Q" + str(j) for i in year_list for j in np.arange(4, 0, -1)]
 
         """
         Creating list of income statement items and their names
         """
         nodes = [rev, cor, gp, opex, ce,
-                 oi,
-                 noi, pti, tax, ni,
+                 oi1,
+                 noi, pti1, tax1, ni,
                  cce5_2,
                  ide1_1,
                  eps, eps_d]
         node_names = ["Revenues", "Cost of Revenue", "Gross Profit", "Operating Expenses", "Cost and Expenses",
                       "Operating Profit"
                      ,"Non-Operating Income/Expense", "Pretax Profit", "Tax", "Net Profit", "Depreciation and Amortization"
                      ,"Interest Expense"
@@ -523,19 +525,19 @@
         """
 
         sic_code = self.SIC
 
         bank_codes = [6022, 6021, 6211, 6029, 6035, 6199]
 
         if sic_code in bank_codes:
-            nodes = [ca2_1, ba1_1, ba1_4,
+            nodes = [ca1_1, ba1_1, ba1_4,
                      ba1_6, ba1_7, ba1_9, ba1_15, ba1_3, ba1_18,
                      ba1_10, nca1_19, ba1_16, ba1_11, a,
                      bl1_1, bl1_3, bl1_9,
-                     cl2_9, bl1_6,
+                     cl1_3, bl1_6,
                      bl1_8, bl1_10, l,
                      se2_3, se2_8, se2_12, se2_11,
                      se1_1, se1_2, se]
 
             node_names = ["Cash and Cash Equivalents", "Securities Purchased Under Agreements to Resell", "Net Loans",
                           "Trading Securities", "Available-For-Sale Securities","Held-To-Maturity Securities", "Derivative Securities", "Securities Borrowed", "Financial Instruments Owned",
                           "Property, Plant and Equipment", "Intangibles", "Accounts Receivables", "Other Assets", "Total Assets",
@@ -543,23 +545,26 @@
                           "Short-Term Debt", "Long-Term Debt",
                           "Accrued Expenses and Accounts Payable", "Other Liabilities", "Total Liabilities",
                           "Common Stock", "Additional Paid In Capital", "Retained Earnings", "Accumulated Other Income",
                           "Stockholder's Equity", "Minority Interest", "Total Equity"]
 
 
         else:
-            nodes = [ca2_1, ca2_2, ca1_4, ca2_12, ca1_34, ca,
-                     nca1_13, nca1_19, nca1_36, nca,
-                     cl2_1, cl2_2, cl1_2, cl1_3, cl1_27, cl,
+            nodes = [ca1_1, ca1_4, ca2_12,
+                     ca1_34, ca1,
+                     nca1_13, nca1_19, nca1_36,
+                     nca,
+                     cl2_1, cl2_2, cl1_2, cl1_3,
+                     cl1_27, cl1,
                      ncl1_1, ncl1_2, ncl,
                      se2_3, se2_8, se2_12, se2_14,
                      se1_1, se1_2,
                      a, l, se]
 
-            node_names = ["Cash and Cash Equivalents", "Short-term Investments", "Accounts Receivable, Net", "Inventories",
+            node_names = ["Cash and Cash Equivalents", "Accounts Receivable, Net", "Inventories",
                           "Other Current Assets", "Total Current Assets",
                           "Property Plant and Equipment", "Intangibles", "Other Non-Current Assets",
                           "Total Non-Current Assets",
                           "Accounts Payable", "Accrued Liabilities", "Deferred Revenue", "Short-term Borrowings",
                           "Other Current Liabilities", "Total Current Liabilities",
                           "Long-Term Debt", "Non-Debt Long Term Liabilities", "Total Non-Current Liabilities",
                           "Capital Stock", "Additional Paid In Capital", "Retained Earnings", "Accumulated Other Change",
@@ -581,22 +586,22 @@
         df.index = df.index.get_level_values(0)
 
         """
         Sense-checking
         """
         if sic_code not in bank_codes:
             df.loc["Total Non-Current Assets"] = df.loc["Total Assets"] - df.loc["Total Current Assets"]
-            df.loc["Other Current Assets"] = df.loc["Total Current Assets"] - df.iloc[0:4].sum()
-            df.loc["Other Non-Current Assets"] = df.loc["Total Non-Current Assets"] - df.iloc[6:7].sum()
+            df.loc["Other Current Assets"] = df.loc["Total Current Assets"] - df.iloc[0:3].sum()
+            df.loc["Other Non-Current Assets"] = df.loc["Total Non-Current Assets"] - df.iloc[5:7].sum()
 
-            df.loc["Other Current Liabilities"] = df.loc["Total Current Liabilities"] - df.iloc[11:15].sum()
+            df.loc["Other Current Liabilities"] = df.loc["Total Current Liabilities"] - df.iloc[9:13].sum()
             df.loc["Total Non-Current Liabilities"] = df.loc["Total Liabilities"] - df.loc["Total Current Liabilities"]
             df.loc["Non-Debt Long Term Liabilities"] = df.loc["Total Non-Current Liabilities"] - df.loc["Long-Term Debt"]
 
-            df.loc["Accumulated Other Change"] = df.loc["Stockholder's Equity"] - df.iloc[19:22].sum()
+            df.loc["Accumulated Other Change"] = df.loc["Stockholder's Equity"] - df.iloc[18:21].sum()
             df.loc["Minority Interest"] = df.loc["Total Equity"] - df.loc["Stockholder's Equity"]
 
         else:
 
             df.loc["Other Assets"] = df.loc["Total Assets"] - df.iloc[0:12].sum()
             df.loc["Other Liabilities"] = df.loc["Total Liabilities"] - df.iloc[14:20].sum()
 
@@ -773,14 +778,15 @@
 ba1_3 = Node("SecuritiesBorrowed", attribute = "debit") # Securities Borrowed
 
 ba1_14 = Node("MarketableSecurities", attribute = "debit") #Marketable Securities
 
 ba1_6 = Node("TradingSecurities", attribute = "debit", parent = ba1_14) #Trading Securities
 
 ba1_15 = Node("DerivativeAssets", attribute = "debit", parent = ba1_14) #Derivative Assets
+ba1_15_1 = Node("DerivativeFinancialAssets", attribute = "debit", parent = ba1_15) #Derivative Assets
 
 ba1_7 = Node("AvailableForSaleSecuritiesDebtSecurities", attribute = "debit", parent = ba1_14) #Available-For-Sale Securities
 ba1_8 = Node("DebtSecuritiesAvailableForSaleExcludingAccruedInterest", attribute = "debit", parent = ba1_7) #Available-For-Sale Securities
 
 ba1_9 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestAfterAllowanceForCreditLoss", attribute = "debit", parent = ba1_14) #Held-To-Maturity Securities
 ba1_17 = Node("DebtSecuritiesHeldToMaturityAmortizedCostAfterAllowanceForCreditLoss", attribute = "debit", parent = ba1_9)
 
@@ -789,14 +795,21 @@
 ba1_11 = Node("OtherAssets", attribute = "debit")
 
 ba1_16 = Node("AccountsReceivableNet", attribute = "debit") # Accounts Receivables
 
 ba1_18 = Node("FinancialInstrumentsOwnedAtFairValue", attribute = "debit") #Financial Instruments Owned
 
 #Level 2
+ba2_22 = Node("LoansAndAdvancesToCustomers", attribute = "debit", parent = ba1_4)
+ba2_23 = Node("LoansAndAdvancesToBanks", attribute = "debit", parent = ba1_4)
+ba2_24 = Node("CorporateLoans", attribute = "debit", parent = ba2_22)
+ba2_25 = Node("ConsumerLoans", attribute = "debit", parent = ba2_22)
+ba2_26 = Node("LoansToGovernment", attribute = "debit", parent = ba2_22)
+
+
 ba2_1 = Node("FederalFundsSold", attribute = "debit", parent = ba1_13)
 ba2_2 = Node("SecuritiesPurchasedUnderAgreementsToResell", attribute = "debit", parent = ba1_13)
 
 ba2_3 = Node("FinancingReceivableAllowanceForCreditLossExcludingAccruedInterest", attribute = "credit", parent = ba1_5)
 ba2_4 = Node("FinancingReceivableAllowanceForCreditLosses", attribute = "credit", parent = ba2_3)
 
 ba2_5 = Node("FinancingReceivableExcludingAccruedInterestBeforeAllowanceForCreditLoss", attribute = "debit", parent = ba1_5)
@@ -808,25 +821,29 @@
 ba2_9 = Node("DebtSecuritiesHeldToMaturityAllowanceForCreditLossExcludingAccruedInterest", attribute = "credit", parent = ba1_17)
 ba2_22 = Node("DebtSecuritiesHeldToMaturityAllowanceForCreditLoss", attribute = "credit", parent = ba2_9)
 ba2_10 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestBeforeAllowanceForCreditLoss", attribute = "debit", parent = ba1_17)
 ba2_21 = Node("HeldToMaturitySecurities", attribute = "debit", parent = ba2_10)
 
 ba2_11 = Node("FinanceLeaseRightOfUseAsset", attribute = "credit", parent = ba1_10)
 ba2_12 = Node("PropertyPlantAndEquipmentNet", attribute = "debit", parent = ba1_10)
+ba2_12_1 = Node("PropertyPlantAndEquipment", attribute = "debit", parent = ba2_12)
 
 ba2_13 = Node("ReceivablesFromCustomers", attribute = "debit", parent = ba1_16)
 ba2_20 = Node("ContractWithCustomerReceivableAfterAllowanceForCreditLossCurrent", attribute = "debit", parent = ba2_13)
 ba2_14 = Node("ReceivablesFromBrokersDealersAndClearingOrganizations", attribute = "debit", parent = ba1_16)
 ba2_15 = Node("AccountsReceivableFromSecuritization", attribute = "debit", parent = ba1_16)
 ba2_16 = Node("AccountsReceivableBilledForLongTermContractsOrPrograms", attribute = "debit", parent = ba1_16)
 ba2_17 = Node("NotesReceivableGross", attribute = "debit", parent = ba1_16)
 ba2_18 = Node("AccruedInvestmentIncomeReceivable", attribute = "debit", parent = ba1_16)
 ba2_19 = Node("PremiumsReceivableAtCarryingValue", attribute = "debit", parent = ba1_16)
 ba2_20 = Node("OtherReceivables", attribute = "debit", parent = ba1_16)
+ba2_30 = Node("TradeAndOtherReceivablesDueFromRelatedParties", attribute = "debit", parent = ba1_16)
+ba2_31 = Node("TradeReceivables", attribute = "debit", parent = ba1_16)
 
+ba2_32 = Node("FinancialAssets", attribute = "debit", parent = ba1_18)
 """
 Banks - Liabilities
 """
 #Level 1
 bl1_1 = Node("FederalFundsPurchasedAndSecuritiesSoldUnderAgreementsToRepurchase", attribute = "credit") #Securities Loaned
 bl1_2 = Node("CarryingValueOfSecuritiesSoldUnderRepurchaseAgreementsAndDepositsReceivedForSecuritiesLoaned", attribute = "credit", parent = bl1_1)
 
@@ -849,17 +866,20 @@
 bl2_2 = Node("SecuritiesSoldUnderAgreementsToRepurchase", attribute = "credit", parent = bl1_2)
 
 bl2_3 = Node("LongTermDebt", attribute = "credit", parent = bl1_6)
 
 bl2_4 = Node("AccountsPayableCurrentAndNoncurrent", attribute = "credit", parent = bl1_8)
 bl2_5 = Node("AccruedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl1_8)
 
+bl2_6 = Node("DepositsFromBanks", attribute = "credit", parent = bl1_3)
+bl2_7 = Node("DepositsFromCustomers", attribute = "credit", parent = bl1_3)
 
 #Level 3
 
+
 bl3_1 = Node("AccruedLiabilitiesAndOtherLiabilities", attribute = "credit", parent = bl2_5)
 bl3_2 = Node("EmployeeRelatedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl2_5)
 bl3_3 = Node("OtherAccruedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl2_5)
 
 bl3_4 = Node("PayablesToCustomers", attribute = "credit", parent = bl2_4)
 bl3_5 = Node("AccountsPayableTradeCurrentAndNoncurrent", attribute = "credit", parent = bl2_4)
 bl3_6 = Node("AccountsPayableInterestBearingCurrentAndNoncurrent", attribute = "credit", parent = bl2_4)
@@ -868,50 +888,53 @@
 
 bl4_1 = Node("AccruedEmployeeBenefitsCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 bl4_2 = Node("AccruedSalariesCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 bl4_3 = Node("WorkersCompensationLiabilityCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 bl4_4 = Node("OtherEmployeeRelatedLiabilitiesCurrentAndNoncurrent", attribute = "credit", parent = bl3_2)
 
 
-
-
 """
 EPS
 """
 
 eps = Node("EarningsPerShareBasic", attribute = "credit")
 eps_d = Node("EarningsPerShareDiluted", attribute = "credit")
 
+eps1 = Node("BasicEarningsLossPerShare", attribute = "credit", parent = eps)
+eps_d1 = Node("DilutedEarningsLossPerShare", attribute = "credit", parent = eps_d)
 """
 Net Income
 """
 
 ni = Node("NetIncomeLoss", attribute="credit")
 
 # Level 1
 ni1_1 = Node("ProfitLoss", attribute="credit", parent=ni)
 
 """
 Pre-tax income
 """
-pti = Node("IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest", attribute="credit", parent=ni)
+pti1 = Node("ProfitLossBeforeTax", attribute="credit", parent=ni1_1) # IFRS
+pti = Node("IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest", attribute="credit", parent=pti1)
 
 # Level 1
 
 pti1_1 = Node("IncomeLossFromContinuingOperationsBeforeIncomeTaxesMinorityInterestAndIncomeLossFromEquityMethodInvestments", attribute="credit", parent=pti)
 
 """
 Tax
 """
-tax = Node("IncomeTaxExpenseBenefit", attribute="debit", parent=ni)
+tax1 = Node("IncomeTaxExpenseContinuingOperations", attribute="debit", parent=ni1_1) #IFRS
+tax = Node("IncomeTaxExpenseBenefit", attribute="debit", parent=tax1)
 
 """
 Operating Income
 """
-oi = Node("OperatingIncomeLoss", attribute="credit", parent=pti1_1)
+oi1 = Node("ProfitLossFromOperatingActivities", attribute="credit", parent=pti1_1) #IFRS
+oi = Node("OperatingIncomeLoss", attribute="credit", parent=oi1)
 
 """
 Gross Profit
 """
 # Level 1
 gp = Node("GrossProfit", attribute="credit", parent=oi)
 
@@ -928,23 +951,26 @@
 rev1_3 = Node("SalesRevenueNet", attribute="credit", parent=rev1_2)
 rev1_4 = Node("SalesRevenueGoodsNet", attribute="credit", parent=rev1_3)
 
 rev1_5 = Node("RegulatedAndUnregulatedOperatingRevenue", attribute="credit", parent=rev1_4)
 
 rev1_6 = Node("RevenuesNetOfInterestExpense", attribute="credit", parent=rev1_5)
 
+rev1_7 = Node("Revenue", attribute = "credit", parent = rev1_6) #IFRS
+
 # Level 2
 
-rev2_1 = Node("NoninterestIncome", attribute="credit", parent=rev1_6)
-rev2_2 = Node("InterestIncomeExpenseNet", attribute="credit", parent=rev1_6)
+rev2_1 = Node("NoninterestIncome", attribute="credit", parent=rev1_7)
+rev2_2 = Node("InterestIncomeExpenseNet", attribute="credit", parent=rev1_7)
 
 """
 Cost of Revenue
 """
-cor = Node("CostOfRevenue", attribute="debit", parent=gp)
+cor = Node("CostOfSales", attribute="debit", parent=gp)
+cor1 = Node("CostOfRevenue", attribute="debit", parent=cor)
 
 # Level 1
 cor1_1 = Node("CostOfGoodsAndServicesSold", attribute="debit", parent=cor)
 cor1_2 = Node("FinancingInterestExpense", attribute="debit", parent=cor)
 cor1_3 = Node("ProvisionForLoanLeaseAndOtherLosses", attribute="debit", parent=cor)
 cor1_4 = Node("PolicyholderBenefitsAndClaimsIncurredNet", attribute="debit", parent=cor)
 cor1_5 = Node("LiabilityForFuturePolicyBenefitsPeriodExpense", attribute="debit", parent=cor)
@@ -1015,15 +1041,16 @@
 cor5_2 = Node("AircraftRental", attribute="debit", parent=cor4_11)
 cor5_3 = Node("LandingFeesAndOtherRentals", attribute="debit", parent=cor4_11)
 
 """
 Operating Expenses
 """
 opex1 = Node("NoninterestExpense", attribute = "debit", parent = oi)
-opex = Node("OperatingExpenses", attribute="debit", parent=opex1)
+opex2 = Node("OperatingExpense", attribute="debit", parent=opex1)
+opex = Node("OperatingExpenses", attribute="debit", parent=opex2)
 
 # Level 1
 opex1_1 = Node("OperatingCostsAndExpenses", attribute="debit", parent=opex)
 opex1_2 = Node("SellingGeneralAndAdministrativeExpense", attribute="debit", parent=opex)
 opex1_3 = Node("ProvisionForDoubtfulAccounts", attribute="debit", parent=opex)
 opex1_4 = Node("OtherGeneralExpense", attribute="debit", parent=opex)
 opex1_5 = Node("GainLossOnDispositionOfAssets1", attribute="debit", parent=opex)
@@ -1379,23 +1406,27 @@
 Liabilities
 """
 l = Node("Liabilities", attribute="credit")
 
 """
 Current Assets
 """
-ca = Node("AssetsCurrent", attribute="debit", parent=a)
+ca1 = Node("CurrentAssets", attribute="debit", parent=a)
+ca = Node("AssetsCurrent", attribute="debit", parent=ca1)
 
 # Level 1
 ca1_1 = Node("CashCashEquivalentsAndShortTermInvestments", attribute="debit", parent=ca)
+ca1_1_1 = Node("CashAndCashEquivalents", attribute="debit", parent=ca1_1)
 ca1_2 = Node("NetInvestmentInLeaseCurrent", attribute="debit", parent=ca)
 ca1_3 = Node("RestrictedCashAndInvestmentsCurrent", attribute="debit", parent=ca)
 
 ca1_4 = Node("ReceivablesNetCurrent", attribute="debit", parent=ca)
 ca1_35 = Node("AccountsAndOtherReceivablesNetCurrent", attribute="debit", parent=ca1_4)
+ca1_35_1 = Node("CurrentReceivablesFromContractsWithCustomers", attribute="debit", parent=ca1_35) #IFRS
+ca1_35_2 = Node("TradeAndOtherCurrentReceivables", attribute="debit", parent=ca1_35_1) #IFRS
 
 ca1_5 = Node("InventoryNetOfAllowancesCustomerAdvancesAndProgressBillings", attribute="debit", parent=ca)
 ca1_6 = Node("PrepaidExpenseCurrent", attribute="debit", parent=ca)
 ca1_7 = Node("ContractWithCustomerAssetNetCurrent", attribute="debit", parent=ca)
 ca1_8 = Node("CapitalizedContractCostNetCurrent", attribute="debit", parent=ca)
 ca1_9 = Node("DeferredCostsCurrent", attribute="debit", parent=ca)
 ca1_10 = Node("DerivativeInstrumentsAndHedges", attribute="debit", parent=ca)
@@ -1421,29 +1452,35 @@
 ca1_30 = Node("AssetsHeldForSaleNotPartOfDisposalGroupCurrent", attribute="debit", parent=ca)
 ca1_31 = Node("DepositsAssetsCurrent", attribute="debit", parent=ca)
 ca1_32 = Node("IntangibleAssetsCurrent", attribute="debit", parent=ca)
 ca1_33 = Node("BusinessCombinationContingentConsiderationAssetCurrent", attribute="debit", parent=ca)
 ca1_34 = Node("OtherAssetsCurrent", attribute="debit", parent=ca)
 
 # Level 2
-ca2_1 = Node("CashAndCashEquivalentsAtCarryingValue", attribute="debit", parent=ca1_1)
-ca2_2 = Node("ShortTermInvestments", attribute="debit", parent=ca1_1)
+ca2_1 = Node("CashAndCashEquivalentsAtCarryingValue", attribute="debit", parent=ca1_1_1)
+ca2_1_1 = Node("Cash", attribute="debit", parent=ca2_1) # IFRS
+ca2_2 = Node("ShortTermInvestments", attribute="debit", parent=ca1_1_1)
+ca2_2_1 = Node("CashEquivalents", attribute="debit", parent=ca2_2) #IFRS
 
 ca2_3 = Node("RestrictedCashAndCashEquivalentsAtCarryingValue", attribute="debit", parent=ca1_3)
 ca2_4 = Node("RestrictedInvestmentsCurrent", attribute="debit", parent=ca1_3)
 ca2_5 = Node("OtherRestrictedAssetsCurrent", attribute="debit", parent=ca1_3)
 
-ca2_6 = Node("AccountsNotesAndLoansReceivableNetCurrent", attribute="debit", parent=ca1_4)
-ca2_7 = Node("NontradeReceivablesCurrent", attribute="debit", parent=ca1_4)
-ca2_8 = Node("UnbilledReceivablesCurrent", attribute="debit", parent=ca1_4)
-ca2_9 = Node("ReceivablesLongTermContractsOrPrograms", attribute="debit", parent=ca1_4)
-ca2_10 = Node("AccountsReceivableFromSecuritization", attribute="debit", parent=ca1_4)
-ca2_11 = Node("OtherReceivablesNetCurrent", attribute="debit", parent=ca1_4)
+ca2_6 = Node("AccountsNotesAndLoansReceivableNetCurrent", attribute="debit", parent=ca1_35_2)
+ca2_7 = Node("NontradeReceivablesCurrent", attribute="debit", parent=ca1_35_2)
+ca2_8 = Node("UnbilledReceivablesCurrent", attribute="debit", parent=ca1_35_2)
+ca2_9 = Node("ReceivablesLongTermContractsOrPrograms", attribute="debit", parent=ca1_35_2)
+ca2_10 = Node("AccountsReceivableFromSecuritization", attribute="debit", parent=ca1_35_2)
+ca2_11 = Node("OtherReceivablesNetCurrent", attribute="debit", parent=ca1_35_2)
+ca2_42 = Node("CurrentTradeReceivables", attribute="debit", parent=ca1_35_2) #IFRS
+ca2_43 = Node("CurrentPrepayments", attribute="debit", parent=ca1_35_2) #IFRS
+ca2_44 = Node("OtherCurrentReceivables", attribute="debit", parent=ca1_35_2) #IFRS
 
 ca2_12 = Node("InventoryNet", attribute="debit", parent=ca1_5)
+ca2_12_1 = Node("Inventories", attribute="debit", parent=ca2_12) #IFRS
 ca2_13 = Node("ProgressPaymentsNettedAgainstInventoryForLongTermContractsOrPrograms", attribute="debit", parent=ca1_5)
 
 ca2_14 = Node("FinancingReceivableExcludingAccruedInterestBeforeAllowanceForCreditLossCurrent", attribute="debit",
               parent=ca1_24)
 ca2_15 = Node("FinancingReceivableAllowanceForCreditLossExcludingAccruedInterestCurrent", attribute="credit",
               parent=ca1_24)
 
@@ -1490,43 +1527,44 @@
 ca2_37 = Node("PrepaidRoyalties", attribute="debit", parent=ca1_6)
 ca2_38 = Node("Supplies", attribute="debit", parent=ca1_6)
 ca2_39 = Node("PrepaidInterest", attribute="debit", parent=ca1_6)
 ca2_40 = Node("PrepaidTaxes", attribute="debit", parent=ca1_6)
 ca2_41 = Node("OtherPrepaidExpenseCurrent", attribute="debit", parent=ca1_6)
 
 # Level 3
-ca3_1 = Node("CashAndDueFromBanks", attribute="debit", parent=ca2_1)
-ca3_2 = Node("InterestBearingDepositsInBanks", attribute="debit", parent=ca2_1)
-ca3_3 = Node("CashEquivalentsAtCarryingValue", attribute="debit", parent=ca2_1)
-
-ca3_4 = Node("EquitySecuritiesFvNi", attribute="debit", parent=ca2_2)
-ca3_5 = Node("DebtSecuritiesCurrent", attribute="debit", parent=ca2_2)
-ca3_6 = Node("MarketableSecuritiesCurrent", attribute="debit", parent=ca2_2)
-ca3_7 = Node("OtherShortTermInvestments", attribute="debit", parent=ca2_2)
+ca3_1 = Node("CashAndDueFromBanks", attribute="debit", parent=ca2_1_1)
+ca3_1_1 = Node("BalancesWithBanks", attribute="debit", parent=ca3_1) #IFRS
+ca3_2 = Node("InterestBearingDepositsInBanks", attribute="debit", parent=ca2_1_1)
+ca3_3 = Node("CashEquivalentsAtCarryingValue", attribute="debit", parent=ca2_1_1)
+
+ca3_4 = Node("EquitySecuritiesFvNi", attribute="debit", parent=ca2_2_1)
+ca3_5 = Node("DebtSecuritiesCurrent", attribute="debit", parent=ca2_2_1)
+ca3_6 = Node("MarketableSecuritiesCurrent", attribute="debit", parent=ca2_2_1)
+ca3_7 = Node("OtherShortTermInvestments", attribute="debit", parent=ca2_2_1)
 
 ca3_8 = Node("RestrictedCashCurrent", attribute="debit", parent=ca2_3)
 ca3_9 = Node("RestrictedCashEquivalentsCurrent", attribute="debit", parent=ca2_3)
 
-ca3_10 = Node("InventoryGross", attribute="debit", parent=ca2_12)
-ca3_11 = Node("InventoryAdjustments", attribute="credit", parent=ca2_12)
+ca3_10 = Node("InventoryGross", attribute="debit", parent=ca2_12_1)
+ca3_11 = Node("InventoryAdjustments", attribute="credit", parent=ca2_12_1)
 
 ca3_12 = Node("AccountsReceivableNetCurrent", attribute="debit", parent=ca2_6)
 ca3_13 = Node("NotesAndLoansReceivableNetCurrent", attribute="credit", parent=ca2_6)
 
 ca3_14 = Node("AllowanceForDoubtfulOtherReceivablesCurrent", attribute="debit", parent=ca2_11)
 ca3_15 = Node("OtherReceivablesGrossCurrent", attribute="credit", parent=ca2_11)
 
 ca3_16 = Node("DeferredGasCost", attribute="debit", parent=ca2_30)
 
 ca3_17 = Node("OtherDeferredCostsGross", attribute="debit", parent=ca2_32)
 ca3_18 = Node("AccumulatedAmortizationOfOtherDeferredCosts", attribute="credit", parent=ca2_32)
 
 # Level 4
-ca4_1 = Node("Cash", attribute="debit", parent=ca3_1)
-ca4_2 = Node("DueFromBanks", attribute="debit", parent=ca3_1)
+ca4_1 = Node("Cash", attribute="debit", parent=ca3_1_1)
+ca4_2 = Node("DueFromBanks", attribute="debit", parent=ca3_1_1)
 
 ca4_3 = Node("TradingSecuritiesDebt", attribute="debit", parent=ca3_5)
 ca4_4 = Node("AvailableForSaleSecuritiesDebtSecuritiesCurrent", attribute="debit", parent=ca3_5)
 ca4_5 = Node("DebtSecuritiesHeldToMaturityAmortizedCostAfterAllowanceForCreditLossCurrent", attribute="debit",
              parent=ca3_5)
 
 ca4_6 = Node("AccountsReceivableGrossCurrent", attribute="debit", parent=ca3_12)
@@ -1599,20 +1637,22 @@
 nca1_7 = Node("DebtSecuritiesHeldToMaturityExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
 nca1_8 = Node("NetInvestmentInLeaseExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
 nca1_9 = Node("DebtSecuritiesAvailableForSaleAmortizedCostExcludingAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
 nca1_10 = Node("LeveragedLeasesNetInvestmentInLeveragedLeasesDisclosureInvestmentInLeveragedLeasesNet", attribute="debit", parent=nca)
 nca1_11 = Node("InventoryRealEstate", attribute="debit", parent=nca)
 nca1_12 = Node("NontradeReceivablesNoncurrent", attribute="debit", parent=nca)
 nca1_13 = Node("PropertyPlantAndEquipmentNet", attribute="debit", parent=nca)
+nca1_13_1 = Node("PropertyPlantAndEquipmentIncludingRightofuseAssets", attribute="debit", parent=nca1_13)
 nca1_14 = Node("PropertyPlantAndEquipmentCollectionsNotCapitalized", attribute="debit", parent=nca)
 nca1_15 = Node("DebtSecuritiesAvailableForSaleAccruedInterestAfterAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca)
 nca1_16 = Node("OilAndGasPropertySuccessfulEffortMethodNet", attribute="debit", parent=nca)
 nca1_17 = Node("OilAndGasPropertyFullCostMethodNet", attribute="debit", parent=nca)
 nca1_18 = Node("LongTermInvestmentsAndReceivablesNet", attribute="debit", parent=nca)
 nca1_19 = Node("IntangibleAssetsNetIncludingGoodwill", attribute="debit", parent=nca)
+nca1_19_1 = Node("IntangibleAssetsAndGoodwill", attribute="debit", parent=nca1_19)
 nca1_20 = Node("PrepaidExpenseNoncurrent", attribute="debit", parent=nca)
 nca1_21 = Node("ContractWithCustomerAssetNetNoncurrent", attribute="debit", parent=nca)
 nca1_22 = Node("CapitalizedContractCostNetNoncurrent", attribute="debit", parent=nca)
 nca1_23 = Node("DerivativeInstrumentsAndHedgesNoncurrent", attribute="debit", parent=nca)
 nca1_24 = Node("RegulatedEntityOtherAssetsNoncurrent", attribute="debit", parent=nca)
 nca1_25 = Node("DepositsAssetsNoncurrent", attribute="debit", parent=nca)
 nca1_26 = Node("DeferredRentReceivablesNetNoncurrent", attribute="debit", parent=nca)
@@ -1663,31 +1703,31 @@
 nca2_22 = Node("IncomeTaxesReceivableNoncurrent", attribute="debit", parent=nca1_12)
 nca2_23 = Node("ValueAddedTaxReceivableNoncurrent", attribute="debit", parent=nca1_12)
 nca2_24 = Node("InsuranceSettlementsReceivableNoncurrent", attribute="debit", parent=nca1_12)
 nca2_25 = Node("GrantsReceivableNoncurrent", attribute="debit", parent=nca1_12)
 nca2_26 = Node("InsuranceReceivableForMalpracticeNoncurrent", attribute="debit", parent=nca1_12)
 nca2_27 = Node("OilAndGasJointInterestBillingReceivablesNoncurrent", attribute="debit", parent=nca1_12)
 
-nca2_28 = Node("PropertyPlantAndEquipmentGross", attribute="debit", parent=nca1_13)
-nca2_29 = Node("AccumulatedDepreciationDepletionAndAmortizationPropertyPlantAndEquipment", attribute="credit",
-               parent=nca1_13)
+nca2_28 = Node("PropertyPlantAndEquipmentGross", attribute="debit", parent=nca1_13_1)
+nca2_28_1 = Node("PropertyPlantAndEquipment", attribute="debit", parent=nca2_28) #IFRS
+nca2_29 = Node("AccumulatedDepreciationDepletionAndAmortizationPropertyPlantAndEquipment", attribute="credit", parent=nca1_13_1)
 
 nca2_30 = Node("OilAndGasPropertySuccessfulEffortMethodGross", attribute="debit", parent=nca1_16)
-nca2_31 = Node("OilAndGasPropertySuccessfulEffortMethodAccumulatedDepreciationDepletionAmortizationAndImpairment",
-               attribute="credit", parent=nca1_16)
+nca2_31 = Node("OilAndGasPropertySuccessfulEffortMethodAccumulatedDepreciationDepletionAmortizationAndImpairment", attribute="credit", parent=nca1_16)
 nca2_32 = Node("OtherOilAndGasPropertySuccessfulEffortMethod", attribute="debit", parent=nca1_16)
 
 nca2_33 = Node("OilAndGasPropertyFullCostMethodGross", attribute="debit", parent=nca1_17)
 nca2_34 = Node("OilAndGasPropertyFullCostMethodDepletion", attribute="credit", parent=nca1_17)
 
 nca2_35 = Node("LongTermInvestments", attribute="debit", parent=nca1_18)
 nca2_36 = Node("LongTermAccountsNotesAndLoansReceivableNetNoncurrent", attribute="debit", parent=nca1_18)
 
-nca2_37 = Node("Goodwill", attribute="debit", parent=nca1_19)
-nca2_38 = Node("IntangibleAssetsNetExcludingGoodwill", attribute="debit", parent=nca1_19)
+nca2_37 = Node("Goodwill", attribute="debit", parent=nca1_19_1)
+nca2_38 = Node("IntangibleAssetsNetExcludingGoodwill", attribute="debit", parent=nca1_19_1)
+nca2_38_1 = Node("IntangibleAssetsOtherThanGoodwill", attribute="debit", parent=nca2_38)
 
 nca2_39 = Node("PrepaidExpenseOtherNoncurrent", attribute="debit", parent=nca1_20)
 nca2_40 = Node("PrepaidMineralRoyaltiesNoncurrent", attribute="debit", parent=nca1_20)
 
 nca2_41 = Node("DerivativeAssetsNoncurrent", attribute="debit", parent=nca1_23)
 nca2_42 = Node("HedgingAssetsNoncurrent", attribute="debit", parent=nca1_23)
 nca2_43 = Node("CommodityContractAssetNoncurrent", attribute="debit", parent=nca1_23)
@@ -1721,24 +1761,24 @@
 nca2_63 = Node("CapitalizedSoftwareDevelopmentCostsForSoftwareSoldToCustomers", attribute="debit", parent=nca1_33)
 nca2_64 = Node("DeferredCompensationPlanAssets", attribute="debit", parent=nca1_33)
 
 nca2_65 = Node("OtherReceivableBeforeAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca1_38)
 nca2_66 = Node("OtherReceivableAllowanceForCreditLossNoncurrent", attribute="debit", parent=nca1_38)
 
 # Level 3
-nca3_1 = Node("LandAndLandImprovements", attribute="debit", parent=nca2_28)
-nca3_2 = Node("BuildingsAndImprovementsGross", attribute="debit", parent=nca2_28)
-nca3_3 = Node("MachineryAndEquipmentGross", attribute="debit", parent=nca2_28)
-nca3_4 = Node("FurnitureAndFixturesGross", attribute="debit", parent=nca2_28)
-nca3_5 = Node("FixturesAndEquipmentGross", attribute="debit", parent=nca2_28)
-nca3_6 = Node("CapitalizedComputerSoftwareGross", attribute="debit", parent=nca2_28)
-nca3_7 = Node("ConstructionInProgressGross", attribute="debit", parent=nca2_28)
-nca3_8 = Node("LeaseholdImprovementsGross", attribute="debit", parent=nca2_28)
-nca3_9 = Node("TimberAndTimberlands", attribute="debit", parent=nca2_28)
-nca3_10 = Node("PropertyPlantAndEquipmentOther", attribute="debit", parent=nca2_28)
+nca3_1 = Node("LandAndLandImprovements", attribute="debit", parent=nca2_28_1)
+nca3_2 = Node("BuildingsAndImprovementsGross", attribute="debit", parent=nca2_28_1)
+nca3_3 = Node("MachineryAndEquipmentGross", attribute="debit", parent=nca2_28_1)
+nca3_4 = Node("FurnitureAndFixturesGross", attribute="debit", parent=nca2_28_1)
+nca3_5 = Node("FixturesAndEquipmentGross", attribute="debit", parent=nca2_28_1)
+nca3_6 = Node("CapitalizedComputerSoftwareGross", attribute="debit", parent=nca2_28_1)
+nca3_7 = Node("ConstructionInProgressGross", attribute="debit", parent=nca2_28_1)
+nca3_8 = Node("LeaseholdImprovementsGross", attribute="debit", parent=nca2_28_1)
+nca3_9 = Node("TimberAndTimberlands", attribute="debit", parent=nca2_28_1)
+nca3_10 = Node("PropertyPlantAndEquipmentOther", attribute="debit", parent=nca2_28_1)
 
 nca3_11 = Node("UnprovedOilAndGasPropertySuccessfulEffortMethod", attribute="debit", parent=nca2_30)
 nca3_12 = Node("ProvedOilAndGasPropertySuccessfulEffortMethod", attribute="debit", parent=nca2_30)
 
 nca3_13 = Node("OilAndGasPropertySuccessfulEffortMethodAccumulatedImpairment", attribute="credit", parent=nca2_31)
 nca3_14 = Node("OilAndGasPropertySuccessfulEffortMethodAccumulatedDepreciationDepletionAndAmortization",
                attribute="credit", parent=nca2_31)
@@ -1792,20 +1832,21 @@
               parent=nca4_5)
 nca5_4 = Node("ConstructionContractorReceivableRetainageAfterYearOne", attribute="debit", parent=nca4_5)
 nca5_5 = Node("ContractReceivableDueAfterOneYear", attribute="debit", parent=nca4_5)
 
 """
 Current Liabilities
 """
-
-cl = Node("LiabilitiesCurrent", attribute="credit", parent=l)
+cl1 = Node("CurrentLiabilities", attribute="credit", parent=l)
+cl = Node("LiabilitiesCurrent", attribute="credit", parent=cl1)
 
 # Level 1
 
 cl1_1 = Node("AccountsPayableAndAccruedLiabilitiesCurrent", attribute="credit", parent=cl)
+cl1_1_1 = Node("CurrentAccrualsAndCurrentDeferredIncomeIncludingCurrentContractLiabilities", attribute = "credit", parent = cl1_1) # IFRS
 cl1_2 = Node("DeferredRevenueCurrent", attribute="credit", parent=cl)
 cl1_3 = Node("DebtCurrent", attribute="credit", parent=cl)
 cl1_4 = Node("DeferredCompensationLiabilityCurrent", attribute="credit", parent=cl)
 cl1_5 = Node("DeferredRentCreditCurrent", attribute="credit", parent=cl)
 cl1_6 = Node("DerivativeInstrumentsAndHedgesLiabilities", attribute="credit", parent=cl)
 cl1_7 = Node("RestructuringReserveCurrent", attribute="credit", parent=cl)
 cl1_8 = Node("LiabilityForUncertainTaxPositionsCurrent", attribute="credit", parent=cl)
@@ -1827,26 +1868,29 @@
 cl1_24 = Node("SelfInsuranceReserveCurrent", attribute="credit", parent=cl)
 cl1_25 = Node("ProgramRightsObligationsCurrent", attribute="credit", parent=cl)
 cl1_26 = Node("BusinessCombinationContingentConsiderationLiabilityCurrent", attribute="credit", parent=cl)
 cl1_27 = Node("OtherLiabilitiesCurrent", attribute="credit", parent=cl)
 
 # Level 2
 
-cl2_1 = Node("AccountsPayableCurrent", attribute="credit", parent=cl1_1)
-cl2_2 = Node("AccruedLiabilitiesCurrent", attribute="credit", parent=cl1_1)
-cl2_3 = Node("EmployeeRelatedLiabilitiesCurrent", attribute="credit", parent=cl1_1)
-cl2_4 = Node("TaxesPayableCurrent", attribute="credit", parent=cl1_1)
-cl2_5 = Node("InterestAndDividendsPayableCurrent", attribute="credit", parent=cl1_1)
-cl2_6 = Node("SettlementLiabilitiesCurrent", attribute="credit", parent=cl1_1)
+cl2_1 = Node("AccountsPayableCurrent", attribute="credit", parent=cl1_1_1)
+cl2_2 = Node("AccruedLiabilitiesCurrent", attribute="credit", parent=cl1_1_1)
+cl2_3 = Node("EmployeeRelatedLiabilitiesCurrent", attribute="credit", parent=cl1_1_1)
+cl2_4 = Node("TaxesPayableCurrent", attribute="credit", parent=cl1_1_1)
+cl2_5 = Node("InterestAndDividendsPayableCurrent", attribute="credit", parent=cl1_1_1)
+cl2_6 = Node("SettlementLiabilitiesCurrent", attribute="credit", parent=cl1_1_1)
 
 cl2_7 = Node("ContractWithCustomerLiabilityCurrent", attribute="credit", parent=cl1_2)
 cl2_8 = Node("DeferredIncomeCurrent", attribute="credit", parent=cl1_2)
 
 cl2_9 = Node("ShortTermBorrowings", attribute="credit", parent=cl1_3)
 cl2_10 = Node("LongTermDebtAndCapitalLeaseObligationsCurrent", attribute="credit", parent=cl1_3)
+cl2_29 = Node("ShorttermBorrowings", attribute="credit", parent=cl1_3)
+cl2_30 = Node("CurrentPortionOfLongtermBorrowings", attribute="credit", parent=cl1_3)
+cl2_31 = Node("CurrentBorrowingsAndCurrentPortionOfNoncurrentBorrowings", attribute="credit", parent=cl1_3)
 
 cl2_11 = Node("DeferredCompensationShareBasedArrangementsLiabilityCurrent", attribute="credit", parent=cl1_4)
 cl2_12 = Node("DeferredCompensationCashBasedArrangementsLiabilityCurrent", attribute="credit", parent=cl1_4)
 cl2_13 = Node("OtherDeferredCompensationArrangementsLiabilityCurrent", attribute="credit", parent=cl1_4)
 
 cl2_14 = Node("DerivativeLiabilitiesCurrent", attribute="credit", parent=cl1_6)
 cl2_15 = Node("EnergyMarketingContractLiabilitiesCurrent", attribute="credit", parent=cl1_6)
@@ -1855,58 +1899,57 @@
 cl2_17 = Node("AccountsPayableRelatedPartiesCurrent", attribute="credit", parent=cl1_19)
 cl2_18 = Node("NotesPayableRelatedPartiesClassifiedCurrent", attribute="credit", parent=cl1_19)
 cl2_19 = Node("DueToEmployeesCurrent", attribute="credit", parent=cl1_19)
 cl2_20 = Node("DueToOfficersOrStockholdersCurrent", attribute="credit", parent=cl1_19)
 cl2_21 = Node("DueToAffiliateCurrentDueToOtherRelatedPartiesClassifiedCurrent", attribute="credit", parent=cl1_19)
 cl2_22 = Node("DueToOtherRelatedPartiesClassifiedCurrent", attribute="credit", parent=cl1_19)
 
-cl2_23 = Node("DisposalGroupIncludingDiscontinuedOperationAccountsPayableAndAccruedLiabilitiesCurrent",
-              attribute="credit", parent=cl1_20)
+cl2_23 = Node("DisposalGroupIncludingDiscontinuedOperationAccountsPayableAndAccruedLiabilitiesCurrent",attribute="credit", parent=cl1_20)
 cl2_24 = Node("DisposalGroupIncludingDiscontinuedOperationDeferredRevenueCurrent", attribute="credit", parent=cl1_20)
 cl2_25 = Node("DisposalGroupIncludingDiscontinuedOperationAccruedIncomeTaxesPayable", attribute="credit", parent=cl1_20)
 cl2_26 = Node("DisposalGroupIncludingDiscontinuedOperationOtherCurrentLiabilities", attribute="credit", parent=cl1_20)
-cl2_27 = Node("DisposalGroupIncludingDiscontinuedOperationPensionPlanBenefitObligationCurrent", attribute="credit",
-              parent=cl1_20)
-cl2_28 = Node("DisposalGroupIncludingDiscontinuedOperationPostretirementPlanBenefitObligationCurrent",
-              attribute="credit", parent=cl1_20)
+cl2_27 = Node("DisposalGroupIncludingDiscontinuedOperationPensionPlanBenefitObligationCurrent", attribute="credit", parent=cl1_20)
+cl2_28 = Node("DisposalGroupIncludingDiscontinuedOperationPostretirementPlanBenefitObligationCurrent", attribute="credit", parent=cl1_20)
 
 # Level 3
 
 cl3_1 = Node("AccountsPayableTradeCurrent", attribute="credit", parent=cl2_1)
 cl3_2 = Node("AccountsPayableInterestBearingCurrent", attribute="credit", parent=cl2_1)
 cl3_3 = Node("ConstructionPayableCurrent", attribute="credit", parent=cl2_1)
 cl3_4 = Node("OilAndGasSalesPayableCurrent", attribute="credit", parent=cl2_1)
 cl3_5 = Node("GasPurchasePayableCurrent", attribute="credit", parent=cl2_1)
 cl3_6 = Node("EnergyMarketingAccountsPayable", attribute="credit", parent=cl2_1)
 cl3_7 = Node("GasImbalancePayableCurrent", attribute="credit", parent=cl2_1)
-cl3_8 = Node("AccountsPayableUnderwritersPromotersAndEmployeesOtherThanSalariesAndWagesCurrent", attribute="credit",
-             parent=cl2_1)
+cl3_8 = Node("AccountsPayableUnderwritersPromotersAndEmployeesOtherThanSalariesAndWagesCurrent", attribute="credit",parent=cl2_1)
 cl3_9 = Node("AccountsPayableOtherCurrent", attribute="credit", parent=cl2_1)
+cl3_63= Node("TradeAndOtherCurrentPayablesToRelatedParties", attribute="credit", parent=cl2_1) #IFRS
+cl3_64= Node("CurrentContractLiabilities", attribute="credit", parent=cl2_1) #IFRS
 
 cl3_10 = Node("AccruedInsuranceCurrent", attribute="credit", parent=cl2_2)
 cl3_11 = Node("AccruedRentCurrent", attribute="credit", parent=cl2_2)
 cl3_12 = Node("AccruedRoyaltiesCurrent", attribute="credit", parent=cl2_2)
 cl3_13 = Node("AccruedUtilitiesCurrent", attribute="credit", parent=cl2_2)
 cl3_14 = Node("AccruedSalesCommissionCurrent", attribute="credit", parent=cl2_2)
 cl3_15 = Node("AccruedProfessionalFeesCurrent", attribute="credit", parent=cl2_2)
 cl3_16 = Node("AccruedAdvertisingCurrent", attribute="credit", parent=cl2_2)
 cl3_17 = Node("AccruedExchangeFeeRebateCurrent", attribute="credit", parent=cl2_2)
 cl3_18 = Node("ProductWarrantyAccrualClassifiedCurrent", attribute="credit", parent=cl2_2)
 cl3_19 = Node("AccruedMarketingCostsCurrent", attribute="credit", parent=cl2_2)
 cl3_20 = Node("OtherAccruedLiabilitiesCurrent", attribute="credit", parent=cl2_2)
+cl3_66 = Node("Accruals", attribute="credit", parent=cl2_2) #IFRS
+cl3_65 = Node("AccrualsClassifiedAsCurrent", attribute="credit", parent=cl2_2) #IFRS
 
 cl3_21 = Node("AccruedSalariesCurrent", attribute="credit", parent=cl2_3)
 cl3_22 = Node("AccruedVacationCurrent", attribute="credit", parent=cl2_3)
 cl3_23 = Node("AccruedBonusesCurrent", attribute="credit", parent=cl2_3)
 cl3_24 = Node("AccruedPayrollTaxesCurrent", attribute="credit", parent=cl2_3)
 cl3_25 = Node("AccruedEmployeeBenefitsCurrent", attribute="credit", parent=cl2_3)
 cl3_26 = Node("WorkersCompensationLiabilityCurrent", attribute="credit", parent=cl2_3)
 cl3_27 = Node("PensionAndOtherPostretirementDefinedBenefitPlansCurrentLiabilities", attribute="credit", parent=cl2_3)
-cl3_28 = Node("PensionAndOtherPostretirementAndPostemploymentBenefitPlansLiabilitiesCurrent", attribute="credit",
-              parent=cl2_3)
+cl3_28 = Node("PensionAndOtherPostretirementAndPostemploymentBenefitPlansLiabilitiesCurrent", attribute="credit", parent=cl2_3)
 cl3_29 = Node("OtherEmployeeRelatedLiabilitiesCurrent", attribute="credit", parent=cl2_3)
 cl3_30 = Node("DefinedBenefitPensionPlanLiabilitiesCurrent", attribute="credit", parent=cl2_3)
 
 cl3_31 = Node("SalesAndExciseTaxPayableCurrent", attribute="credit", parent=cl2_4)
 cl3_32 = Node("AccruedIncomeTaxesCurrent", attribute="credit", parent=cl2_4)
 cl3_33 = Node("AccrualForTaxesOtherThanIncomeTaxesCurrent", attribute="credit", parent=cl2_4)
 
@@ -1943,14 +1986,16 @@
 cl3_60 = Node("FederalHomeLoanBankAdvancesCurrent", attribute="credit", parent=cl2_10)
 
 cl3_61 = Node("DisposalGroupIncludingDiscontinuedOperationAccountsPayableCurrent", attribute="credit", parent=cl2_23)
 cl3_62 = Node("DisposalGroupIncludingDiscontinuedOperationAccruedLiabilitiesCurrent", attribute="credit", parent=cl2_23)
 
 # Level 4
 
+cl4_6 = Node("CurrentAdvances", attribute = "credit", parent = cl3_64)
+
 cl4_1 = Node("StandardProductWarrantyAccrualCurrent", attribute="credit", parent=cl3_18)
 cl4_2 = Node("ExtendedProductWarrantyAccrualCurrent", attribute="credit", parent=cl3_18)
 
 cl4_3 = Node("TaxCutsAndJobsActOf2017TransitionTaxForAccumulatedForeignEarningsLiabilityCurrent", attribute="credit",
              parent=cl3_32)
 
 cl4_4 = Node("NotesPayableCurrent", attribute="credit", parent=cl3_58)
@@ -1969,19 +2014,20 @@
 cl5_8 = Node("OtherLoansPayableCurrent", attribute="credit", parent=cl4_5)
 
 """
 Non-Current Liabilties
 """
 
 ncl = Node("LiabilitiesNoncurrent", attribute="credit", parent=l)
+ncl1 = Node("NoncurrentLiabilities", attribute="credit", parent=ncl)
 
 # Level 1
 
-ncl1_1 = Node("LongTermDebtAndCapitalLeaseObligations", attribute="credit", parent=ncl)
-ncl1_2 = Node("LiabilitiesOtherThanLongtermDebtNoncurrent", attribute="credit", parent=ncl)
+ncl1_1 = Node("LongTermDebtAndCapitalLeaseObligations", attribute="credit", parent=ncl1)
+ncl1_2 = Node("LiabilitiesOtherThanLongtermDebtNoncurrent", attribute="credit", parent=ncl1)
 
 # Level 2
 
 ncl2_1 = Node("LongTermDebtNoncurrent", attribute="credit", parent=ncl1_1)
 ncl2_2 = Node("CapitalLeaseObligationsNoncurrent", attribute="credit", parent=ncl1_1)
 
 ncl2_3 = Node("LiabilitiesOtherThanLongtermDebtNoncurrent", attribute="credit", parent=ncl1_2)
@@ -1994,20 +2040,20 @@
 ncl3_4 = Node("SecuredLongTermDebt", attribute="credit", parent=ncl2_1)
 ncl3_5 = Node("SubordinatedLongTermDebt", attribute="credit", parent=ncl2_1)
 ncl3_6 = Node("UnsecuredLongTermDebt", attribute="credit", parent=ncl2_1)
 ncl3_7 = Node("ConvertibleDebtNoncurrent", attribute="credit", parent=ncl2_1)
 ncl3_8 = Node("ConvertibleSubordinatedDebtNoncurrent", attribute="credit", parent=ncl2_1)
 ncl3_9 = Node("LongTermTransitionBond", attribute="credit", parent=ncl2_1)
 ncl3_10 = Node("LongTermPollutionControlBond", attribute="credit", parent=ncl2_1)
-ncl3_11 = Node("JuniorSubordinatedDebentureOwedToUnconsolidatedSubsidiaryTrustNoncurrent", attribute="credit",
-               parent=ncl2_1)
+ncl3_11 = Node("JuniorSubordinatedDebentureOwedToUnconsolidatedSubsidiaryTrustNoncurrent", attribute="credit", parent=ncl2_1)
 ncl3_12 = Node("LongTermNotesAndLoans", attribute="credit", parent=ncl2_1)
 ncl3_13 = Node("SpecialAssessmentBondNoncurrent", attribute="credit", parent=ncl2_1)
 ncl3_14 = Node("LongtermFederalHomeLoanBankAdvancesNoncurrent", attribute="credit", parent=ncl2_1)
 ncl3_15 = Node("OtherLongTermDebtNoncurrent", attribute="credit", parent=ncl2_1)
+ncl3_45 = Node("LongtermBorrowings", attribute="credit", parent=ncl2_1)
 
 ncl3_16 = Node("AccountsPayableAndAccruedLiabilitiesNoncurrent", attribute="credit", parent=ncl2_3)
 ncl3_17 = Node("DeferredRevenueNoncurrent", attribute="credit", parent=ncl2_3)
 ncl3_18 = Node("DeferredCompensationLiabilityClassifiedNoncurrent", attribute="credit", parent=ncl2_3)
 ncl3_19 = Node("AccumulatedDeferredInvestmentTaxCredit", attribute="credit", parent=ncl2_3)
 ncl3_20 = Node("DeferredGainOnSaleOfProperty", attribute="credit", parent=ncl2_3)
 ncl3_21 = Node("DeferredRentCreditNoncurrent", attribute="credit", parent=ncl2_3)
@@ -2137,34 +2183,40 @@
 te1_5 = Node("RedeemableNoncontrollingInterestEquityOtherCarryingAmount", attribute="credit", parent=te1_2)
 
 """
 Stockholder's Equity
 """
 
 se = Node("StockholdersEquityIncludingPortionAttributableToNoncontrollingInterest", attribute="credit")
-
+se1 = Node("Equity", attribute="credit", parent=se)
 # Level 1
-se1_1 = Node("StockholdersEquity", attribute="credit", parent=se)
-se1_2 = Node("MinorityInterest", attribute="credit", parent=se)
+
+se1_1 = Node("StockholdersEquity", attribute="credit", parent=se1)
+se1_2 = Node("MinorityInterest", attribute="credit", parent=se1)
 
 # Level 2
 se2_1 = Node("PreferredStockValue", attribute="credit", parent=se1_1)
 se2_2 = Node("PreferredStockSharesSubscribedButUnissuedSubscriptionsReceivable", attribute="debit", parent=se1_1)
 se2_3 = Node("CommonStockValue", attribute="credit", parent=se1_1)
+se2_27 = Node("IssuedCapital", attribute="credit", parent=se2_3) #IFRS
 se2_4 = Node("TreasuryStockValue", attribute="debit", parent=se1_1)
 se2_5 = Node("CommonStockHeldBySubsidiary", attribute="debit", parent=se1_1)
 se2_6 = Node("CommonStockShareSubscribedButUnissuedSubscriptionsReceivable", attribute="debit", parent=se1_1)
 se2_7 = Node("CommonStockSharesSubscriptions", attribute="credit", parent=se1_1)
 se2_8 = Node("AdditionalPaidInCapital", attribute="credit", parent=se1_1)
+se2_28 = Node("SharePremium", attribute="credit", parent=se2_8) #IFRS
 se2_9 = Node("TreasuryStockDeferredEmployeeStockOwnershipPlan", attribute="credit", parent=se1_1)
 se2_10 = Node("DeferredCompensationEquity", attribute="debit", parent=se1_1)
 se2_11 = Node("AccumulatedOtherComprehensiveIncomeLossNetOfTax", attribute="credit", parent=se1_1)
+se2_30 = Node("AccumulatedOtherComprehensiveIncome", attribute="credit", parent=se2_11)
 se2_12 = Node("RetainedEarningsAccumulatedDeficit", attribute="credit", parent=se1_1)
+se2_26 = Node("RetainedEarnings", attribute="credit", parent=se2_12) #IFRS
 se2_13 = Node("UnearnedESOPShares", attribute="debit", parent=se1_1)
 se2_14 = Node("OtherAdditionalCapital", attribute="credit", parent=se1_1)
+se2_29 = Node("OtherReserves", attribute="credit", parent=se2_14) #IFRS
 se2_15 = Node("ReceivableFromOfficersAndDirectorsForIssuanceOfCapitalStock", attribute="debit", parent=se1_1)
 se2_16 = Node("ReceivableFromShareholdersOrAffiliatesForIssuanceOfCapitalStock", attribute="debit", parent=se1_1)
 se2_17 = Node("WarrantsAndRightsOutstanding", attribute="credit", parent=se1_1)
 se2_18 = Node("StockholdersEquityNoteSubscriptionsReceivable", attribute="debit", parent=se1_1)
 
 se2_19 = Node("MinorityInterestInLimitedPartnerships", attribute="credit", parent=se1_2)
 se2_20 = Node("MinorityInterestInOperatingPartnerships", attribute="credit", parent=se1_2)
@@ -2188,16 +2240,16 @@
 se3_7 = Node("AociLossCashFlowHedgeCumulativeGainLossAfterTax", attribute="credit", parent=se2_11)
 se3_8 = Node("AccumulatedOtherComprehensiveIncomeLossDefinedBenefitPensionAndOtherPostretirementPlansNetOfTax",
              attribute="debit", parent=se2_11)
 se3_9 = Node("AccumulatedOtherComprehensiveIncomeLossFinancialLiabilityFairValueOptionAfterTax", attribute="credit",
              parent=se2_11)
 se3_10 = Node("AociDerivativeQualifyingAsHedgeExcludedComponentAfterTax", attribute="credit", parent=se2_11)
 
-se3_11 = Node("RetainedEarningsAppropriated", attribute="credit", parent=se2_12)
-se3_12 = Node("RetainedEarningsUnappropriated", attribute="credit", parent=se2_12)
+se3_11 = Node("RetainedEarningsAppropriated", attribute="credit", parent=se2_26)
+se3_12 = Node("RetainedEarningsUnappropriated", attribute="credit", parent=se2_26)
 
 # Level 4
 se4_1 = Node("DefinedBenefitPlanAccumulatedOtherComprehensiveIncomeNetGainsLossesAfterTax", attribute="credit",
              parent=se3_8)
 se4_2 = Node("DefinedBenefitPlanAccumulatedOtherComprehensiveIncomeNetPriorServiceCostCreditAfterTax",
              attribute="debit", parent=se3_8)
 se4_3 = Node("DefinedBenefitPlanAccumulatedOtherComprehensiveIncomeNetTransitionAssetsObligationsAfterTax",
@@ -2210,45 +2262,50 @@
 cce = Node("CashAndCashEquivalentsPeriodIncreaseDecrease", attribute="debit")
 
 
 # End-cash position
 cce1 = Node("CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents", attribute="debit")
 cce2 = Node("CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations", attribute="debit", parent=cce1)
 cce3 = Node("CashAndCashEquivalentsAtCarryingValue", attribute="debit", parent=cce2)
+cce4 = Node("CashAndCashEquivalents", attribute="debit", parent=cce3)
 
 # Level 1
 
 cce1_1 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations", attribute="debit", parent=cce)
 cce1_3 = Node("EffectOfExchangeRateOnCashAndCashEquivalents", attribute="debit", parent=cce1_1)
+cce1_4 = Node("EffectOfExchangeRateChangesOnCashAndCashEquivalents", attribute="debit", parent=cce1_3)
 
 cce1_2 = Node("CashAndCashEquivalentsPeriodIncreaseDecreaseExcludingExchangeRateEffect", attribute="debit", parent=cce)
 
 # Level 2
 
-cce2_1 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents", attribute="debit", parent=cce1_3)
+cce2_1 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents", attribute="debit", parent=cce1_4)
 cce2_2 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsDisposalGroupIncludingDiscontinuedOperations", attribute="debit", parent=cce2_1)
 
 cce2_3 = Node("NetCashProvidedByUsedInOperatingActivities", attribute="debit", parent=cce1_2)
+cce2_3_1 = Node("CashFlowsFromUsedInOperatingActivities", attribute="debit", parent=cce2_3)
 cce2_4 = Node("NetCashProvidedByUsedInInvestingActivities", attribute="debit", parent=cce1_2)
+cce2_4_1 = Node("CashFlowsFromUsedInInvestingActivities", attribute="debit", parent=cce2_4)
 cce2_5 = Node("NetCashProvidedByUsedInFinancingActivities", attribute="debit", parent=cce1_2)
+cce2_5_1 = Node("CashFlowsFromUsedInFinancingActivities", attribute="debit", parent=cce2_5)
 
 # Level 3
 
 cce3_7 = Node("EffectOfExchangeRateOnCashAndCashEquivalentsContinuingOperations", attribute="debit", parent=cce2_2)
 cce3_8 = Node("EffectOfExchangeRateOnCashAndCashEquivalentsDiscontinuedOperations", attribute="debit", parent=cce2_2)
 
-cce3_1 = Node("ProfitLoss", attribute="debit", parent=cce2_3)
+cce3_1 = Node("ProfitLoss", attribute="debit", parent=cce2_3_1)
 cce3_2 = Node("AdjustmentsToReconcileNetIncomeLossToCashProvidedByUsedInOperatingActivities", attribute="debit",
-              parent=cce2_3)
+              parent=cce2_3_1)
 
-cce3_3 = Node("NetCashProvidedByUsedInInvestingActivitiesContinuingOperations", attribute="debit", parent=cce2_4)
-cce3_4 = Node("CashProvidedByUsedInInvestingActivitiesDiscontinuedOperations", attribute="debit", parent=cce2_4)
+cce3_3 = Node("NetCashProvidedByUsedInInvestingActivitiesContinuingOperations", attribute="debit", parent=cce2_4_1)
+cce3_4 = Node("CashProvidedByUsedInInvestingActivitiesDiscontinuedOperations", attribute="debit", parent=cce2_4_1)
 
-cce3_5 = Node("NetCashProvidedByUsedInFinancingActivitiesContinuingOperations", attribute="debit", parent=cce2_5)
-cce3_6 = Node("CashProvidedByUsedInFinancingActivitiesDiscontinuedOperations", attribute="debit", parent=cce2_5)
+cce3_5 = Node("NetCashProvidedByUsedInFinancingActivitiesContinuingOperations", attribute="debit", parent=cce2_5_1)
+cce3_6 = Node("CashProvidedByUsedInFinancingActivitiesDiscontinuedOperations", attribute="debit", parent=cce2_5_1)
 
 # Level 4
 
 cce4_1 = Node("IncomeLossIncludingPortionAttributableToNoncontrollingInterest", attribute="credit", parent=cce3_1)
 cce4_2 = Node("IncomeTaxExpenseBenefitContinuingOperationsDiscontinuedOperationsExtraordinaryItems", attribute="debit",
               parent=cce3_1)
 
@@ -2261,35 +2318,39 @@
 cce4_8 = Node("PaymentsForProceedsFromProductiveAssets", attribute="credit", parent=cce3_3)
 
 # level 5
 
 cce5_1 = Node("PaymentsToAcquireProductiveAssets", attribute="credit", parent=cce4_8)
 
 cce5_2 = Node("DepreciationDepletionAndAmortization", attribute="debit", parent=cce4_3)
+cce5_2_1 = Node("DepreciationAndAmortisationExpense", attribute = "debit", parent = cce5_2) #IFRS
+cce5_2_2 = Node("DepreciationAmortisationAndImpairmentLossReversalOfImpairmentLossRecognisedInProfitOrLoss", attribute = "debit", parent = cce5_2_1) #IFRS
 
 # Level 6
 
 cce6_1 = Node("PaymentsToAcquirePropertyPlantAndEquipment", attribute="credit", parent=cce5_1)
 
-cce6_2 = Node("DepreciationAndAmortization", attribute="debit", parent=cce5_2)
-cce6_3 = Node("Depletion", attribute="debit", parent=cce5_2)
+cce6_2 = Node("DepreciationAndAmortization", attribute="debit", parent=cce5_2_2)
+cce6_3 = Node("Depletion", attribute="debit", parent=cce5_2_2)
 
 # Level 7
 cce7_1 = Node("PaymentsToAcquireAndDevelopRealEstate", attribute="credit", parent=cce6_1)
 cce7_2 = Node("PaymentsToAcquireFurnitureAndFixtures", attribute="credit", parent=cce6_1)
 cce7_3 = Node("PaymentsToAcquireMachineryAndEquipment", attribute="credit", parent=cce6_1)
 cce7_4 = Node("PaymentsToAcquireOilAndGasPropertyAndEquipment", attribute="credit", parent=cce6_1)
 cce7_5 = Node("PaymentsToExploreAndDevelopOilAndGasProperties", attribute="credit", parent=cce6_1)
 cce7_6 = Node("PaymentsToAcquireMiningAssets", attribute="credit", parent=cce6_1)
 cce7_7 = Node("PaymentsToAcquireTimberlands", attribute="credit", parent=cce6_1)
 cce7_8 = Node("PaymentsToAcquireWaterAndWasteWaterSystems", attribute="credit", parent=cce6_1)
 cce7_9 = Node("PaymentsToAcquireOtherPropertyPlantAndEquipment", attribute="credit", parent=cce6_1)
 
 cce7_10 = Node("Depreciation", attribute="debit", parent=cce6_2)
+cce7_14 = Node("DepreciationExpense", attribute="debit", parent=cce7_10) #IFRS
 cce7_11 = Node("AdjustmentForAmortization", attribute="debit", parent=cce6_2)
+cce7_15 = Node("AmortisationExpense", attribute="debit", parent=cce7_11) #IFRS
 cce7_12 = Node("AmortizationOfDeferredCharges", attribute="debit", parent=cce6_2)
 cce7_13 = Node("OtherDepreciationAndAmortization", attribute="debit", parent=cce6_2)
 
 # Level 8
 
 cce8_1 = Node("PaymentsToAcquireRealEstate", attribute="credit", parent=cce7_1)
 cce8_2 = Node("PaymentsToDevelopRealEstateAssets", attribute="credit", parent=cce7_1)
@@ -2297,21 +2358,21 @@
 
 cce8_4 = Node("PaymentsToAcquireOilAndGasProperty", attribute="credit", parent=cce7_4)
 cce8_5 = Node("PaymentsToAcquireOilAndGasEquipment", attribute="credit", parent=cce7_4)
 
 cce8_6 = Node("PaymentsToAcquireWaterSystems", attribute="credit", parent=cce7_8)
 cce8_7 = Node("PaymentsToAcquireWasteWaterSystems", attribute="credit", parent=cce7_8)
 
-cce8_8 = Node("CostOfGoodsSoldDepreciation", attribute="debit", parent=cce7_10)
-cce8_9 = Node("CostOfServicesDepreciation", attribute="debit", parent=cce7_10)
-cce8_10 = Node("DepreciationNonproduction", attribute="debit", parent=cce7_10)
-
-cce8_11 = Node("CostOfServicesAmortization", attribute="debit", parent=cce7_11)
-cce8_12 = Node("AmortizationOfIntangibleAssets", attribute="debit", parent=cce7_11)
-cce8_13 = Node("CostOfGoodsSoldAmortization", attribute="debit", parent=cce7_11)
+cce8_8 = Node("CostOfGoodsSoldDepreciation", attribute="debit", parent=cce7_14)
+cce8_9 = Node("CostOfServicesDepreciation", attribute="debit", parent=cce7_14)
+cce8_10 = Node("DepreciationNonproduction", attribute="debit", parent=cce7_14)
+
+cce8_11 = Node("CostOfServicesAmortization", attribute="debit", parent=cce7_15)
+cce8_12 = Node("AmortizationOfIntangibleAssets", attribute="debit", parent=cce7_15)
+cce8_13 = Node("CostOfGoodsSoldAmortization", attribute="debit", parent=cce7_15)
 
 # Level 9
 
 cce9_1 = Node("PaymentsForDepositsOnRealEstateAcquisitions", attribute="credit", parent=cce8_1)
 cce9_2 = Node("PaymentsToAcquireCommercialRealEstate", attribute="credit", parent=cce8_1)
 cce9_3 = Node("PaymentsToAcquireBuildings", attribute="credit", parent=cce8_1)
 cce9_4 = Node("PaymentsForCapitalImprovements", attribute="credit", parent=cce8_1)
```

### Comparing `finqual-1.0.0/finqual.egg-info/PKG-INFO` & `finqual-1.1.0/finqual.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
-Author: Myztika
+Author: Harry
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -79,21 +79,21 @@
 
 The `ratios` function calculates selected financial ratios for the specified timeframe and returns the mean average over that timeframe. The selected financial ratios are a selection of liquidity, profitability and valuation ratios, which are commonly used to compare against other companies,
 
 The `comparables` function returns a list of `n` comparable companies based on the SIC code of the initialized ticker (i.e. companies in the same industry as the chosen company). The comparable companies are selected based on market capitalisation, and users can adjust the optional input `level` to determine the number of SIC digits to consider, whereby level takes an integer from 1 to 4, with 4 being the default and the most granular industry classification possible within the package.
 
 ## Dependencies
 
-Only four packages are required, with the following versions confirmed to be working:
+Only five packages are required, with the following versions confirmed to be working:
 
 | Package   | Version   |
 |-----------|-----------|
 | pandas    | >= 2.0.2  |
 | numpy     | >= 1.24.3 |
 | requests  | >= 2.28.1 |
 | ratelimit | >= 2.2.1  |
 | datetime  | >= 5.1    |
 
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
-- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database
+- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database or use the IFRS taxonomy instead of the US GAAP taxonomy
```

