---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: ExtendedFieldURI 要素は、拡張 MAPI プロパティを識別します。
ms.openlocfilehash: 8d946aec8ae2c5e6bb4ca3f1d8ee74250262d373
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760403"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

**ExtendedFieldURI**要素は、拡張 MAPI プロパティを識別します。 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

 **PathToExtendedFieldType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |よく知られている定義プロパティは、拡張 MAPI プロパティの Id を設定します。  <br/> この属性を使用する場合、 **PropertySetId**と**PropertyTag**の属性は使用できません。 **PropertyId**または**プロパティ名**のいずれかの属性、および**登録するとき**の属性とは、この属性を使用する必要があります。  <br/> このトピックの後半の**DistinguishedPropertySetId**の属性テーブルは、この属性の可能な値を示します。  <br/> この属性は、省略可能です。  <br/> |
|**PropertySetId** <br/> |プロパティ セットまたは名前空間を識別する GUID で拡張 MAPI を識別します。  <br/> この属性を使用する場合、 **DistinguishedPropertySetId**と**PropertyTag**の属性は使用できません。 **PropertyId**または**プロパティ名**のいずれかの属性、および**登録するとき**の属性とは、この属性を使用する必要があります。  <br/> この属性は、省略可能です。  <br/> |
|**PropertyTag** <br/> |タグの型部分のないプロパティ タグを識別します。 **PropertyTag**は、16 進数または短整数のいずれかとして表すことができます。  <br/> 0x8000 から 0 xfffe までの間では、プロパティのカスタム範囲を表します。 メールボックス データベースでは、最初にカスタム プロパティを検出すると、0x8000-0 xfffe のカスタム プロパティ範囲内のプロパティ タグがそのカスタム プロパティで割り当てられます。 指定されたカスタム プロパティ タグは、データベース間でほとんどの場合によって異なります。 したがって、プロパティ タグによるカスタム プロパティ要求は異なるデータベースに異なるプロパティを返すことができます。 カスタム プロパティには、 **PropertyTag**属性の使用は禁止されています。 代わりに、 **PropertySetId**属性と**プロパティ名**または**PropertyId**属性を使用します。  <br/> > [!IMPORTANT]> 0x8000 から 0 xfffe までの任意のカスタム プロパティの GUID と名前と id。 を使用してアクセスします。           **PropertyTag**属性を使用する場合は、 **DistinguishedPropertySetId**、 **PropertySetId**、**プロパティ名**、および**PropertyId**属性を使用できません。  <br/> この属性は、省略可能です。  <br/> > [!NOTE]> 0x8000-0 xfffe のユーザー設定の範囲内のプロパティのプロパティ タグの属性は使用できません。 ここでは名前付きプロパティを使用する必要があります。           |
|**PropertyName** <br/> |名前を使用して拡張プロパティを識別します。 このプロパティは、 **DistinguishedPropertySetId**または**PropertySetId**のいずれかに結合する必要があります。  <br/> この属性を使用する場合、 **PropertyId**および**PropertyTag**属性は使用できません。  <br/> この属性は、省略可能です。  <br/> |
|**PropertyId** <br/> |拡張プロパティをそのディスパッチ ID を識別します。 10 進または 16 進数のいずれかの形式では、ディスパッチ ID を識別できます。 このプロパティは、 **DistinguishedPropertySetId**または**PropertySetId**のいずれかに結合する必要があります。  <br/> この属性を使用する場合、**プロパティ名**と**PropertyTag**の属性は使用できません。  <br/> この属性は、省略可能です。  <br/> |
|**登録するとき** <br/> |プロパティ タグのプロパティ型を表します。 これは、プロパティ タグの最下位ワードに対応しています。  <br/> このトピックで後で登録するときの属性テーブルには、この属性の有効な値が含まれています。  <br/> この属性は、必要があります。  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>DistinguishedPropertySetId 属性

|**値**|**説明**|
|:-----|:-----|
|会議  <br/> |会議を識別するプロパティは、名前で ID を設定します。  <br/> |
|Appointment  <br/> |予定のプロパティ セット ID を名前で識別します。  <br/> |
|Common  <br/> |名前で共通のプロパティ セット ID を識別します。  <br/> |
|PublicStrings  <br/> |パブリック文字列のプロパティ セット ID を名前で識別します。  <br/> |
|Address  <br/> |名前によるアドレスのプロパティ セット ID を識別します。  <br/> |
|InternetHeaders  <br/> |インターネット ヘッダーのプロパティ セット ID を名前で識別します。  <br/> |
|CalendarAssistant  <br/> |予定表のアシスタントのプロパティ セット ID を名前で識別します。  <br/> |
|UnifiedMessaging  <br/> |名前によって、ユニファイド メッセージングのプロパティ セット ID を識別します。  <br/> |
   
#### <a name="propertytype-attribute"></a>属性を登録するとき

|**値**|**説明**|
|:-----|:-----|
|ApplicationTime  <br/> |Double 型の値、日付と時刻として解釈されます。 日付は、整数部と小数部は時刻をです。  <br/> |
|ApplicationTimeArray  <br/> |日付と時刻として解釈される 2 つの値の配列。  <br/> |
|バイナリ型 (Binary)  <br/> |Base64 エンコードのバイナリ値です。  <br/> |
|BinaryArray  <br/> |Base64 エンコードのバイナリ値の配列。  <br/> |
|ブール型  <br/> |ブール値**true**または**false を指定**します。  <br/> |
|CLSID  <br/> |GUID 文字列です。  <br/> |
|CLSIDArray  <br/> |GUID の文字列の配列。  <br/> |
|通貨型 (Currency)  <br/> |セントの値として解釈される 64 ビット整数。  <br/> |
|CurrencyArray  <br/> |セントの値として解釈される 64 ビット整数の配列。  <br/> |
|倍精度浮動小数点型 (Double)  <br/> |64 ビットの浮動小数点値です。  <br/> |
|DoubleArray  <br/> |64 ビット浮動小数点値の配列。  <br/> |
|エラー  <br/> |SCODE の値です。32 ビット符号なし整数。  <br/> 制限、または値を取得または設定は使用されません。 これは、レポート用にのみ存在します。  <br/> |
|浮動小数点型 (Float)  <br/> |32 ビットの浮動小数点値です。  <br/> |
|FloatArray  <br/> |32 ビット浮動小数点値の配列。  <br/> |
|整数型 (Integer)  <br/> |符号付き 32 ビット (Int32) 整数。  <br/> |
|IntegerArray  <br/> |符号付き 32 ビット (Int32) 整数の配列。  <br/> |
|Long 型 (Long)  <br/> |符号付きまたは符号なし 64 ビット (Int64) 整数。  <br/> |
|LongArray  <br/> |符号付きまたは符号なしの 64 ビット (Int64) 整数の配列。  <br/> |
|Null  <br/> |プロパティの値がないことを示します。  <br/> 制限、または値を取得または設定は使用されません。 これは、レポート用にのみ存在します。  <br/> |
|オブジェクト  <br/> |IUnknown インターフェイスを実装するオブジェクトへのポインター。  <br/> 制限、または値を取得または設定は使用されません。 これは、レポート用にのみ存在します。  <br/> |
|ObjectArray  <br/> |IUnknown インターフェイスを実装するオブジェクトへのポインターの配列。  <br/> 制限、または値を取得または設定は使用されません。 これは、レポート用にのみ存在します。  <br/> |
|長い形式の日付 (スラッシュ区切り)  <br/> |符号付き 16 ビット整数。  <br/> |
|ShortArray  <br/> |16 ビット符号付き整数の配列。  <br/> |
|SystemTime  <br/> |FILETIME 構造体の形式で 64 ビットの整数データと時刻値。  <br/> |
|SystemTimeArray  <br/> |FILETIME 構造体の形式で 64 ビット整数のデータと時刻の値の配列。  <br/> |
|String  <br/> |Unicode 文字列です。  <br/> |
|自己責任で使用  <br/> |Unicode 文字列の配列。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーおよびアイテムの拡張プロパティを識別します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | 追加のプロパティを識別します。  <br/>  この要素への XPath 式は、次のように。  <br/>  `/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中にアイテムから指定されたプロパティを削除する削除操作を表します。  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |UpdateFolder の呼び出し中にフォルダーから特定のプロパティを削除する削除操作を表します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。  <br/> |
|[存在します。](exists.md) <br/> |**True**を返す指定されたプロパティが存在する場合、アイテムの検索式を表します。  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |プロパティまたは別のプロパティを比較するときに使用する定数値のいずれかを表します。  <br/> |
|[IsEqualTo](isequalto.md) <br/> |プロパティを定数値または別のプロパティを比較し、これらが等しい場合**は true**に評価する検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |最初のプロパティ値が大きい場合、プロパティ、定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |最初のプロパティには、もう 1 つ以上の場合は、プロパティ、定数値または別プロパティは、返す**場合は true**を比較するための検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティが以下の場合に**true**を返す検索式を表す 2 番目の。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティが以下の場合に**true**を返す検索式を表す 2 番目の。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |値が同じではない場合、プロパティを定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。  <br/> |
|[除外](excludes.md) <br/> |プロパティのビットごとのマスクを実行します。  <br/> |
|[内容](contains.md) <br/> |指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。  <br/> |
|[FieldOrder](fieldorder.md) <br/> |結果の並べ替えに使用する単一のフィールドを表し、並べ替えの方向を示します。  <br/> |
   
## <a name="remarks"></a>備考

いくつかの属性は、他の属性と組み合わせて使用できません。 拡張プロパティの属性の無効な組み合わせが付属しているすべての要求は、エラー メッセージが生成されます。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
> [!NOTE]
> Microsoft .net では、long 型の値は、64 ビット符号付き整数の MAPI と COM、long 型の値は、32 ビット整数。 ほとんどの開発者は、Exchange Web サービス クライアント アプリケーションを開発するのに着眼点フレームワークを使用します。 MAPI ではなく .NET の名前付けの使用、名前を付けます。 、0x0E07、PR_MESSAGE_FLAGS の MAPI プロパティは、PT_LONG 型です。 .NET では、整数値と見なされます。 として PR_MESSAGE_FLAGS の拡張プロパティが定義されている\<t:ExtendedFieldURI PropertyTag ="0x0E07"PropertyType =「整数」と\>。 
  
## <a name="example"></a>例

要求の次の例では、2 つのカスタム プロパティを持つアイテムを作成します。 最初のカスタム プロパティを**true**に設定するブール値を持つ**IsMyHouse**と呼びます。 2 番目のユーザー設定の拡張プロパティを" **HousePrices**を"といいます。 通貨の値の配列が含まれています。 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
    MessageDisposition="SaveOnly">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </SavedItemFolderId>
      <Items>
        <t:Item>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Create an extended property</t:Subject>
          <t:Body BodyType="Text">Added info to extended props</t:Body>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="IsMyHouse" 
                                PropertyType="Boolean"/>
            <t:Value>true</t:Value>
          </t:ExtendedProperty>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="HousePrices" 
                                PropertyType="CurrencyArray"/>
            <t:Values>
              <t:Value>30000000</t:Value>
              <t:Value>40000000</t:Value>
              <t:Value>50000000</t:Value>
            </t:Values>
          </t:ExtendedProperty>
        </t:Item>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[FieldURI](fielduri.md)
  
[IndexedFieldURI](indexedfielduri.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

