---
title: Exchange で EWS とともに検索フィルターを使用する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: EWS マネージ API または Exchange の EWS によって検索ファイルを使用する方法を確認します。
localization_priority: Priority
ms.openlocfilehash: 04a74ec92d4bced8abd58d164a1c186d6405e679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455836"
---
# <a name="use-search-filters-with-ews-in-exchange"></a>Exchange で EWS とともに検索フィルターを使用する

EWS マネージ API または Exchange の EWS によって検索ファイルを使用する方法を確認します。
  
検索フィルターは、EWS Managed API または EWS アプリケーションで検索条件を記述するための主要なツールです。[クエリ文字列](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)ではなく、検索フィルターを使用して以下を実行することをお勧めします。
  
- 特定のプロパティまたはプロパティのセットを検索します。  
- 複数の検索条件を使用して検索します。
    
検索フィルターは、次のいずれかを実行する場合、唯一のオプションです。
  
- カスタム プロパティを検索します。  
- 大文字小文字を区別して文字列の検索を実行します。  
- プレフィックスまたは完全に一致する文字列の検索を実行します。 
- ビットマスクの検索を実行します。
- 値に関係なく特定のプロパティ セットを持つアイテムを検索します。
- フォルダーを検索します。
- 検索フォルダーを作成します。
    
## <a name="determine-what-type-of-search-filter-you-need"></a>必要な検索フィルターの種類を決定します。
<a name="bk_SelectFilter"> </a>

検索フィルターを作成する前に、まず必要なフィルターの種類を決定します。 フィルターの種類は、EWS マネージ API では [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) クラスの子クラスとして、EWS では [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) 要素の子要素として実装されます。 
  
**表 1. 検索フィルターの種類**

|**フィルターの種類**|**EWS マネージ API のクラス**|**EWS の要素**|**説明**|
|:-----|:-----|:-----|:-----|
|包含フィルター  <br/> |[ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |文字列比較に使用するのに最適なフィルターの種類です。大文字小文字の区別、空白を無視するかどうかを制御でき、包含モードを設定できます。  <br/> |
|ビットマスク フィルター  <br/> |[ExcludesBitmask](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[Excludes](https://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |整数のプロパティをビットマスクとして検索し、指定されたビットマスクに対応するビットが設定されていない結果のみを返すことができます。  <br/> |
|存在フィルター  <br/> |[Exists](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[Exists](https://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |値に関係なく指定したプロパティを持つすべてのアイテムを返します。  <br/> |
|等値フィルター  <br/> |[IsEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [IsNotEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[IsEqualTo](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [IsNotEqualTo](https://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |指定された定数値または別のプロパティの値のいずれかを持つ、指定されたプロパティの値を比較し、**IsEqualTo** フィルターの場合は同じ値を持つすべてのアイテムを返し、**IsNotEqualTo** フィルターの場合は非等値を返します。  <br/> |
|関係テスト フィルター  <br/> |[IsGreaterThan](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [IsGreaterThanOrEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [IsLessThan](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [IsLessThanOrEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[IsGreaterThan](https://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [IsGreaterThanOrEqualTo](https://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [IsLessThan](https://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [IsLessThanOrEqualTo](https://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |指定された定数値または別のプロパティのいずれかに該当する関係において、指定したプロパティの値を持つすべてのアイテムを返します。 たとえば、**IsGreaterThan** フィルターは指定されたプロパティの指定された値よりも大きい値を持つすべてのアイテムを返します。  <br/> |
|否定フィルター  <br/> |[Not](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[Not](https://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |他のフィルターの結果を否定します。  <br/> |
|複合フィルター  <br/> |[SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[And](https://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [Or](https://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |複数のフィルターを組み合わせて複雑な検索条件を指定できます。  <br/> |
   
### <a name="contains-filter"></a>包含フィルター

包含フィルターは、文字列のプロパティを検索するための最適な選択肢です。包含フィルターを使用すると、包含モードと比較モードを設定することによって、大文字小文字の区別や空白の処理方法など、文字列の一致のさまざまな面を制御することができます。
  
#### <a name="contains-filter-in-the-ews-managed-api"></a>EWS マネージ API での包含フィルター
<a name="bk_ContainsEWSMA"> </a>

EWS マネージ API を使用している場合、[ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) クラスの [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) プロパティを使用して包含モードを設定し、**ContainsSubstring** クラスの [ComparisonMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) プロパティを使用して比較モードを設定します。 次の例では、"meeting notes" (会議メモ) という部分文字列を、アイテムの件名フィールドで検索する検索フィルターを作成する方法を示します。 この例では大文字と小文字は無視されますが、空白は無視されません。 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a>EWS での包含フィルター
<a name="bk_ContainsEWSMA"> </a>

EWS では、[Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) 要素の **ContainmentMode** 属性を使用して包含モードを設定し、**Contains** 要素の **ContainmentComparison** 属性を使用して比較モードを設定します。 次の例では、"meeting notes" (会議メモ) という部分文字列を、アイテムの件名フィールドで検索するための検索フィルターを作成する方法を示します。 この例では大文字と小文字は無視されますが、空白は無視されません。 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a>ビットマスク フィルター

ビットマスク フィルターを使用すると、整数のプロパティをビットマスクとして検索し、指定されたプロパティの値に特定のビットが設定されていない結果を返すことができます。
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a>EWS マネージ API でのビットマスク フィルター

次の例では、EWS マネージ API を使用して、(この記事の「[例: 検索フィルターと EWS マネージ API を使用してアイテムを検索する](#bk_ExampleEWSMA)」セクションで定義された) **ItemIndex** カスタム プロパティの値を持ち、2 番目のビット (バイナリの 10) が設定されていないすべてのアイテムを返す検索フィルターを作成する方法を示します。 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a>EWS でのビットマスク フィルター

次の例では、EWS を使用して、(この記事の「[例: 検索フィルターと EWS マネージ API を使用してアイテムを検索する](#bk_ExampleEWSMA)」セクションで定義された) **ItemIndex** カスタム プロパティの値を持ち、2 番目のビット (バイナリの 10) が設定されていないすべてのアイテムを返す検索フィルターを作成する方法を示します。 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a>存在フィルター

存在フィルターを使用すると、値に関係なく特定のプロパティが設定されているアイテムを検索できます。
  
#### <a name="exists-filter-in-the-ews-managed-api"></a>EWS マネージ API での存在フィルター

次の例は、**ItemIndex** カスタム プロパティが設定されているすべてのアイテムを返す検索フィルターを作成する方法を示しています。 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a>EWS での存在フィルター

次の例は、**ItemIndex** カスタム プロパティが設定されているすべてのアイテムを返す検索フィルターを作成する方法を示しています。 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a>等値フィルター

等値フィルターでは、特定の値に等しいか、特定の値に等しくない、指定されたプロパティの値を持つすべてのアイテムを検索できます。比較する値は、定数値、またはアイテムごとの別のプロパティの値のいずれかにできます。
  
#### <a name="equality-filter-in-the-ews-managed-api"></a>EWS Managed API での等値フィルター

次の例は、EWS Managed API を使用して、読み取られていないすべてのアイテムを返す検索フィルターを作成する方法を示しています。
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

次の例は、アイテムのサイズに等しくない **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示しています。 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a>EWS での等値フィルター

次の例は、EWS を使用して、読み取られていないすべてのアイテムを返す検索フィルターを作成する方法を示しています。
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

次の例は、アイテムのサイズに等しくない **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示しています。 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a>関係テスト フィルター

関係テスト フィルターでは、指定された値より大きい (\>)、指定された値以上である (\>=)、指定された値より小さい (\<)、または指定された値以下である (\<=) 指定したプロパティの値を持つすべてのアイテムを検索できます。 比較する値は、定数値、またはアイテムごとの別のプロパティの値のいずれかにできます。
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a>EWS マネージ API での関係テスト フィルター

次の例では、EWS Managed API を使用して、定数値 3 に対して指定された関係である **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a>EWS での関係テスト フィルター

次の例では、EWS を使用して、定数値 3 よりも大きい **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

次の例では、定数値 3 以上の **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

次の例では、定数値 3 よりも小さい **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

次の例では、定数値 3 以下の **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a>否定フィルター

否定フィルターでは、別のフィルターを否定し、反対の検索結果を得ることができます。他のフィルターは特定の条件に一致する結果を返すのに対し、否定フィルターは、適用されるフィルターで指定した条件に一致しない結果を返します。
  
#### <a name="negating-filter-in-the-ews-managed-api"></a>EWS Managed API での否定フィルター

次の例は、EWS Managed API を使用して、件名に部分文字列 "meeting notes" (会議メモ) を持たないすべてのアイテムを返す検索フィルターを作成する方法を示しています。
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a>EWS での否定フィルター

次の例は、件名に部分文字列 "meeting notes" (会議メモ) を持たないすべてのアイテムを返す検索フィルターを作成する方法を示しています。
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a>複合フィルター

複合フィルターでは、複数のフィルターを組み合わせてより複雑な検索条件を作成することができます。 論理演算子 AND または OR を使用して、条件を組み合わせることができます。 この方法で、「件名に ’meeting notes’ (会議メモ) が含まれている Sadie Daniels からすべてのメール」のような検索を行うことができます。
  
#### <a name="compound-filter-in-the-ews-managed-api"></a>EWS マネージ API での複合フィルター

次の例では、EWS Managed API を使用して、Sadie Daniels から送信され、件名に "meeting notes" (会議メモ) を含むすべてのアイテムを返す検索フィルターを作成する方法を示しています。
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a>EWS での複合フィルター

次の例では、EWS を使用して、Sadie Daniels から送信され、件名に "meeting notes" (会議メモ) を含むすべてのアイテムを返す検索フィルターを作成する方法を示しています。
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a>例: 検索フィルターと EWS マネージ API を使用してアイテムを検索する
<a name="bk_ExampleEWSMA"> </a>

次の EWS マネージ API メソッドは検索フィルターを使用します。
  
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
次の例では **ExchangeService.FindItems** メソッドを使用しますが、同じルールと概念がすべてのメソッドに適用されます。 この例では、**SearchWithFilter** というメソッドが定義されています。 パラメーターとして、[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト、[WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) オブジェクト、および [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) オブジェクトを取ります。 この例では、**ExchangeService** オブジェクトは [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。 **SearchFilter** クラスは、さまざまな検索フィルターすべての基本クラスです。 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

この記事の例で示すあらゆる検索フィルターに、この関数を使用できます。この例では、複合フィルターを使用して、件名に "meeting notes" (会議メモ) がある Sadie Daniels からの受信トレイのすべてのアイテムを返します。
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a>例: 検索フィルターと EWS を使用してアイテムを検索する
<a name="bk_ExampleEWS"> </a>

次の EWS の操作は検索フィルターを使用します。
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
次の例では **FindItem** 操作を使用しますが、両方の操作で同じルールと概念が適用されます。 検索フィルターは、SOAP 要求の [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) 要素に含まれます。 この例では、前述の EWS マネージ API の例で示している検索に相当する SOAP 要求を送信します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

次の例は、検索結果を含むサーバーからの応答を示しています。
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>次の手順
<a name="bk_ExampleEWS"> </a>

これで、基本的な検索での検索フィルターの使用に慣れ、より高度な検索テクニックに進むことができます。
  
- [Exchange で EWS を使用して、グループ化された検索を実行する](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用してページング検索を実行する](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の検索と EWS](search-and-ews-in-exchange.md)    
- [Exchange で EWS を使用して AQS 検索を実行する](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [FindFolder 操作](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

