# Comparing `tmp/ynab_transaction_adjuster-1.2.0.tar.gz` & `tmp/ynab_transaction_adjuster-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_transaction_adjuster-1.2.0.tar", max compression
+gzip compressed data, was "ynab_transaction_adjuster-1.3.0.tar", max compression
```

## Comparing `ynab_transaction_adjuster-1.2.0.tar` & `ynab_transaction_adjuster-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    35148 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/LICENSE
--rw-r--r--   0        0        0     3421 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/README.md
--rw-r--r--   0        0        0      696 2024-04-28 06:43:23.459809 ynab_transaction_adjuster-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      291 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/__init__.py
--rw-r--r--   0        0        0     6369 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/adjuster.py
--rw-r--r--   0        0        0     2954 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/client.py
--rw-r--r--   0        0        0     1003 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/exceptions.py
--rw-r--r--   0        0        0      357 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/__init__.py
--rw-r--r--   0        0        0      246 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/category.py
--rw-r--r--   0        0        0      621 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/categorygroup.py
--rw-r--r--   0        0        0      263 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/credentials.py
--rw-r--r--   0        0        0     2927 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiedtransaction.py
--rw-r--r--   0        0        0     1718 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifier.py
--rw-r--r--   0        0        0     1252 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiersubtransaction.py
--rw-r--r--   0        0        0      586 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/payee.py
--rw-r--r--   0        0        0      594 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/subtransaction.py
--rw-r--r--   0        0        0     3106 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/transaction.py
--rw-r--r--   0        0        0       72 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/__init__.py
--rw-r--r--   0        0        0     1980 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/categoryrepo.py
--rw-r--r--   0        0        0     1771 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/payeerepo.py
--rw-r--r--   0        0        0     2848 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/serializer.py
--rw-r--r--   0        0        0     1283 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/signaturechecker.py
--rw-r--r--   0        0        0     4262 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3503 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/README.md
+-rw-r--r--   0        0        0      696 2024-04-30 05:09:10.324808 ynab_transaction_adjuster-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      313 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/__init__.py
+-rw-r--r--   0        0        0     6792 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/adjuster.py
+-rw-r--r--   0        0        0     3527 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/client.py
+-rw-r--r--   0        0        0     1118 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/exceptions.py
+-rw-r--r--   0        0        0      386 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/account.py
+-rw-r--r--   0        0        0      246 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/category.py
+-rw-r--r--   0        0        0      621 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/categorygroup.py
+-rw-r--r--   0        0        0      319 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/credentials.py
+-rw-r--r--   0        0        0     2982 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/modifiedtransaction.py
+-rw-r--r--   0        0        0     1878 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/modifier.py
+-rw-r--r--   0        0        0     1252 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/modifiersubtransaction.py
+-rw-r--r--   0        0        0      586 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/payee.py
+-rw-r--r--   0        0        0      594 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/subtransaction.py
+-rw-r--r--   0        0        0     3323 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/transaction.py
+-rw-r--r--   0        0        0      109 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/repos/__init__.py
+-rw-r--r--   0        0        0     1223 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/repos/accountrepo.py
+-rw-r--r--   0        0        0     1980 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/repos/categoryrepo.py
+-rw-r--r--   0        0        0     1771 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/repos/payeerepo.py
+-rw-r--r--   0        0        0     2848 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/serializer.py
+-rw-r--r--   0        0        0     1283 2024-04-30 05:08:55.296717 ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/signaturechecker.py
+-rw-r--r--   0        0        0     4344 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-1.3.0/PKG-INFO
```

### Comparing `ynab_transaction_adjuster-1.2.0/LICENSE` & `ynab_transaction_adjuster-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/README.md` & `ynab_transaction_adjuster-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 		# your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
 ### Initialize
-Create a `Credentials` object and initialize Adjuster class with it
+Create a `Credentials` object and initialize Adjuster class with it. Providing `account` for the credentials is 
+optional. If not set the Adjuster will work on all transactions in the budget.  
 ```py
 from ynabtransactionadjuster import Credentials
 
 my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
 my_adjuster = MyAdjuster(my_credentials)
 ```
 
@@ -71,10 +72,9 @@
 modified_transactions = my_adjuster.apply()
 ```
 
 ### Update
 The modified transactions can be upated in YNAB passing them to the `update()` function. The method returns an integer 
 with the number of successfully updated records.
 ```py
-modified_transactions = my_adjuster.apply()
 count_of_updated_transactions = my_adjuster.update(modified_transactions)
 ```
```

### Comparing `ynab_transaction_adjuster-1.2.0/pyproject.toml` & `ynab_transaction_adjuster-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynab-transaction-adjuster"
-version = "1.2.0"
+version = "1.3.0"
 description = "Library to adjust transactions in YNAB based on custom patterns"
 authors = ["Daniel Basta <ynab@basta.info>"]
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabtransactionadjuster'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/adjuster.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/adjuster.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,48 +6,59 @@
 from ynabtransactionadjuster.models import ModifiedTransaction
 from ynabtransactionadjuster.models.credentials import Credentials
 from ynabtransactionadjuster.client import Client
 from ynabtransactionadjuster.models import Transaction
 from ynabtransactionadjuster.models import Modifier
 from ynabtransactionadjuster.repos import CategoryRepo
 from ynabtransactionadjuster.repos import PayeeRepo
+from ynabtransactionadjuster.repos.accountrepo import AccountRepo
 from ynabtransactionadjuster.serializer import Serializer
 from ynabtransactionadjuster.signaturechecker import SignatureChecker
 
 
 class Adjuster(metaclass=ABCMeta):
 	"""Abstract class which modifies transactions according to concrete implementation. You need to create your own
 	child class and implement the `filter()`and `adjust()` method in it according to your needs. It has attributes
 	which allow you to lookup categories and payees from your budget.
 
 	:ivar categories: Collection of current categories in YNAB budget
 	:ivar payees: Collection of current payees in YNAB budget
+	:ivar accounts: Collection of current accounts in YNAB budget
 	:ivar transactions: All current non deleted transactions from YNAB Account
 	:ivar credentials: Credentials for YNAB API
 	"""
 	def __init__(self, credentials: Credentials):
 		self.credentials = credentials
 		self._client = Client.from_credentials(self.credentials)
 		self._categories = None
 		self._payees = None
+		self._accounts = None
 
 	@property
 	def categories(self) -> CategoryRepo:
 		if not self._categories:
 			self._categories = CategoryRepo(self._client.fetch_categories())
 		return self._categories
 
 	@property
 	def payees(self) -> PayeeRepo:
 		if not self._payees:
 			self._payees = PayeeRepo(self._client.fetch_payees())
 		return self._payees
 
 	@property
+	def accounts(self) -> AccountRepo:
+		if not self._accounts:
+			self._accounts = AccountRepo(self._client.fetch_accounts())
+		return self._accounts
+
+	@property
 	def transactions(self) -> List[Transaction]:
+		if self.credentials.account:
+			return self._client.fetch_transactions(account_id=self.credentials.account)
 		return self._client.fetch_transactions()
 
 	@abstractmethod
 	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
 		"""Function which implements filtering for the list of transactions from YNAB account. It receives a list of
 		the original transactions which can be filtered. Must return the filtered list or just the list if no filtering
 		is intended.
```

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/client.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import requests
 from requests import HTTPError
 
 from ynabtransactionadjuster.models import CategoryGroup, ModifiedTransaction
 from ynabtransactionadjuster.models import Transaction
 from ynabtransactionadjuster.models import Payee
+from ynabtransactionadjuster.models.account import Account
 from ynabtransactionadjuster.models.credentials import Credentials
 
 YNAB_BASE_URL = 'https://api.ynab.com/v1'
 
 
 class Client:
 	"""Client for reading from and writing to YNAB
@@ -42,17 +43,30 @@
 		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/payees', headers=self._header)
 		r.raise_for_status()
 
 		data = r.json()['data']['payees']
 		payees = [Payee.from_dict(p) for p in data if p['deleted'] is False]
 		return payees
 
-	def fetch_transactions(self) -> List[Transaction]:
-		"""Fetches transactions from YNAB"""
-		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/accounts/{self._account}/transactions', headers=self._header)
+	def fetch_accounts(self) -> List[Account]:
+		"""Fetches accounts from YNAB"""
+		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/accounts', headers=self._header)
+		r.raise_for_status()
+
+		data = r.json()['data']['accounts']
+		accounts = [Account(name=a['name'], id=a['id']) for a in data if a['deleted'] is False]
+		return accounts
+
+	def fetch_transactions(self, account_id: str = None) -> List[Transaction]:
+		"""Fetches transactions from YNAB
+
+		:param account_id: Optional YNAB account ID to fetch only for specific account
+		"""
+		account_part_url = f'accounts/{account_id}/' if account_id else ''
+		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/{account_part_url}transactions', headers=self._header)
 		r.raise_for_status()
 
 		data = r.json()['data']['transactions']
 		transaction_dicts = [t for t in data if t['deleted'] is False]
 		transactions = [Transaction.from_dict(t) for t in transaction_dicts]
 		return transactions
```

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/exceptions.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,7 +25,11 @@
 	"""Raised when an error occurs while running the factory on a transaction or during validation of the returned
 	results of the run"""
 	pass
 
 
 class SignatureError(Exception):
 	""" Raised when function is not defined with right signature"""
+
+
+class NoMatchingAccountError(Exception):
+	"""Raised when no matching account is found in the specified budget"""
```

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/categorygroup.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/categorygroup.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiedtransaction.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/modifiedtransaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 	def as_dict(self) -> dict:
 		"""Returns a dictionary representation of the transaction which is used for the update call to YNAB"""
 		t_dict = dict(id=self.transaction.id,
 					  payee_name=self.modifier.payee.name,
 					  payee_id=self.modifier.payee.id,
 					  date=datetime.strftime(self.modifier.transaction_date, '%Y-%m-%d'),
 					  approved=self.modifier.approved,
-					  cleared=self.modifier.cleared)
+					  cleared=self.modifier.cleared,
+					  account_id=self.modifier.account.id)
 		if len(self.modifier.subtransactions) > 0:
 			t_dict['subtransactions'] = [s.as_dict() for s in self.modifier.subtransactions]
 		if self.modifier.category:
 			t_dict['category_id'] = self.modifier.category.id
 		if self.modifier.flag_color:
 			t_dict['flag_color'] = self.modifier.flag_color
 		if self.modifier.memo:
@@ -42,15 +43,15 @@
 		return t_dict
 
 	@property
 	def changed_attributes(self) -> dict:
 		"""Returns a dictionary representation of the modified values and the original transaction"""
 		changed_attributes = dict()
 
-		for a in ('payee', 'category', 'flag_color', 'memo', 'approved', 'cleared'):
+		for a in ('payee', 'category', 'flag_color', 'memo', 'approved', 'cleared', 'account'):
 			if self._attribute_changed(a):
 				changed_attributes[a] = self._create_changed_dict(a)
 
 		if (self.modifier.transaction_date.isocalendar() !=
 				self.transaction.transaction_date.isocalendar()):
 			changed_attributes['transaction_date'] = self._create_changed_dict('transaction_date')
```

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifier.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/modifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,47 +2,51 @@
 from datetime import date
 from typing import List, Literal, Optional
 
 from ynabtransactionadjuster.models import Category
 from ynabtransactionadjuster.models import Transaction
 from ynabtransactionadjuster.models import ModifierSubTransaction
 from ynabtransactionadjuster.models import Payee
+from ynabtransactionadjuster.models.account import Account
 
 
 class Modifier(BaseModel):
 	"""Transaction object prefilled with values from original transaction which can take modified values
 
 	:ivar category: The category of the transaction
 	:ivar transaction_date: The date of the transaction
 	:ivar memo: The memo of the transaction
 	:ivar payee: The payee of the transaction
 	:ivar flag_color: The flag color of the transaction
 	:ivar subtransactions: The subtransactions of the transaction
 	:ivar cleared: Clearance status
 	:ivar approved: Approval status of the transaction
+	:ivar account: The account of the transaction
 	"""
 
 	transaction_date: date
 	category: Optional[Category]
 	memo: Optional[str]
 	payee: Payee
 	flag_color: Optional[Literal['red', 'green', 'blue', 'orange', 'purple', 'yellow']]
 	subtransactions: List[ModifierSubTransaction]
 	approved: bool
 	cleared: Literal['uncleared', 'cleared', 'reconciled']
+	account: Account
 
 	@classmethod
 	def from_transaction(cls, transaction: Transaction):
 		return cls(transaction_date=transaction.transaction_date,
 				   category=transaction.category,
 				   payee=transaction.payee,
 				   memo=transaction.memo,
 				   flag_color=transaction.flag_color,
 				   approved=transaction.approved,
 				   cleared=transaction.cleared,
-				   subtransactions=[])
+				   subtransactions=[],
+				   account=transaction.account)
 
 	@model_validator(mode='after')
 	def check_values(self):
 		if len(self.subtransactions) == 1:
 			raise ValueError(f"There must be at least two subtransactions for a split")
 		return self
```

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiersubtransaction.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/modifiersubtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/payee.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/payee.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/subtransaction.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/subtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/transaction.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/models/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from dataclasses import dataclass, asdict
 from datetime import date, datetime
 from typing import Literal, Optional, Tuple
 
+from ynabtransactionadjuster.models.account import Account
 from ynabtransactionadjuster.models.category import Category
 from ynabtransactionadjuster.models.payee import Payee
 from ynabtransactionadjuster.models.subtransaction import SubTransaction
 
 
 @dataclass(frozen=True, eq=True)
 class Transaction:
 	"""Represents original transaction from YNAB
 
-	:ivar id: The original transaction id
+	:ivar id: The transaction id
+	:ivar account: The account of the transaction
 	:ivar amount: The transaction amount in milliunits format
 	:ivar category: The category of the original transaction
 	:ivar transaction_date: The date of the original transaction
 	:ivar memo: The memo of the original transaction
 	:ivar payee: The payee of the original transaction
 	:ivar flag_color: The flag color of the original transaction
 	:ivar import_payee_name: The payee as recorded by YNAB on import
 	:ivar import_payee_name_original: The original payee or memo as recorded by the bank
 	:ivar approved: approval status of the original transaction
 	:ivar cleared: clearance state of the original transaction
 	:ivar transfer_transaction_id: id of the originating transaction if transaction is transfer
 	"""
 	id: str
+	account: Account
 	transaction_date: date
 	category: Optional[Category]
 	amount: int
 	memo: Optional[str]
 	payee: Payee
 	flag_color: Optional[Literal['red', 'green', 'blue', 'orange', 'purple', 'yellow']]
 	import_payee_name_original: Optional[str]
@@ -52,14 +55,15 @@
 		def build_subtransaction(s_dict: dict) -> SubTransaction:
 			return SubTransaction(payee=build_payee(s_dict),
 								  category=build_category(s_dict),
 								  amount=s_dict['amount'],
 								  memo=s_dict['memo'])
 
 		return Transaction(id=t_dict['id'],
+						   account=Account(id=t_dict['account_id'], name=t_dict['account_name']),
 						   transaction_date=datetime.strptime(t_dict['date'], '%Y-%m-%d').date(),
 						   category=build_category(t_dict),
 						   memo=t_dict['memo'],
 						   import_payee_name_original=t_dict['import_payee_name_original'],
 						   import_payee_name=t_dict['import_payee_name'],
 						   flag_color=t_dict['flag_color'],
 						   payee=build_payee(t_dict),
@@ -69,8 +73,8 @@
 						   cleared=t_dict['cleared'],
 						   transfer_transaction_id=t_dict['transfer_transaction_id'])
 
 	def as_dict(self) -> dict:
 		return asdict(self)
 
 	def __str__(self) -> str:
-		return f"{self.transaction_date} | {self.payee.name} | {float(self.amount) / 1000:.2f} | {self.memo}"
+		return f"{self.account.name} | {self.transaction_date} | {self.payee.name} | {float(self.amount) / 1000:.2f} | {self.memo}"
```

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/categoryrepo.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/repos/categoryrepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/payeerepo.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/repos/payeerepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/serializer.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/serializer.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/signaturechecker.py` & `ynab_transaction_adjuster-1.3.0/ynabtransactionadjuster/signaturechecker.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.2.0/PKG-INFO` & `ynab_transaction_adjuster-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-transaction-adjuster
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library to adjust transactions in YNAB based on custom patterns
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -73,15 +73,16 @@
 		# your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
 ### Initialize
-Create a `Credentials` object and initialize Adjuster class with it
+Create a `Credentials` object and initialize Adjuster class with it. Providing `account` for the credentials is 
+optional. If not set the Adjuster will work on all transactions in the budget.  
 ```py
 from ynabtransactionadjuster import Credentials
 
 my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
 my_adjuster = MyAdjuster(my_credentials)
 ```
 
@@ -93,11 +94,10 @@
 modified_transactions = my_adjuster.apply()
 ```
 
 ### Update
 The modified transactions can be upated in YNAB passing them to the `update()` function. The method returns an integer 
 with the number of successfully updated records.
 ```py
-modified_transactions = my_adjuster.apply()
 count_of_updated_transactions = my_adjuster.update(modified_transactions)
 ```
```

