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
ms.openlocfilehash: fd365010016c68236107991717ed538c97dc0d50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526033"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

**ExtendedFieldURI**要素は、拡張 MAPI プロパティを識別します。 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |拡張 MAPI プロパティの既知のプロパティセット Id を定義します。<br/><br/>この属性を使用する場合、 **Propertysetid**属性と**propertysetid**属性は使用できません。 この属性は、 **PropertyId**属性または**PropertyName**属性、 **recordtype**属性のいずれかで使用する必要があります。<br/><br/>このトピックの後半の**DistinguishedPropertySetId**属性の表に、この属性に指定できる値を示します。<br/><br/>この属性は省略可能です。  <br/> |
|**PropertySetId** <br/> |MAPI 拡張プロパティセットまたは名前空間を識別する GUID で識別します。<br/><br/>この属性を使用する場合、 **DistinguishedPropertySetId**および**propertytag**属性を使用することはできません。 この属性は、 **PropertyId**属性または**PropertyName**属性、 **recordtype**属性のいずれかで使用する必要があります。<br/><br/>この属性は省略可能です。  <br/> |
|**PropertyTag** <br/> |タグの種類の部分がないプロパティタグを識別します。 **Propertytag**は、16進数または短整数のいずれかの形式で表すことができます。<br/><br/>0x8000 ~ 0xFFFE の範囲は、プロパティのユーザー設定範囲を表します。 メールボックスデータベースが初めてカスタムプロパティを検出すると、そのカスタムプロパティが0xFFFE のカスタムプロパティ範囲内にプロパティタグとして割り当てられます。 指定したカスタムプロパティタグは、データベースごとに異なる可能性があります。 そのため、プロパティタグによってカスタムプロパティを取得すると、データベースごとに異なるプロパティを返すことができます。 **Propertytag**属性の使用は、カスタムプロパティでは禁止されています。 代わりに、 **Propertysetid**属性と**PropertyName**属性または**PropertyId**属性を使用します。<br/><br/>**重要**: GUID + NAME/ID を使用して、0X8000 ~ 0xFFFE の任意のカスタムプロパティにアクセスできます。 **Propertytag**属性が使用されている場合、 **DistinguishedPropertySetId**、 **propertytag**、 **PropertyName**、および**PropertyId**属性は使用できません。<br/><br/>この属性は省略可能です。<br/><br/>**注**: カスタム範囲 0X8000 ~ 0xFFFE 内のプロパティに対して、プロパティタグ属性を使用することはできません。 この場合は、名前付きプロパティを使用する必要があります。           |
|**PropertyName** <br/> |名前によって拡張プロパティを識別します。 このプロパティは、 **DistinguishedPropertySetId**または**propertysetid**と組み合わせて使用する必要があります。<br/><br/>この属性を使用する場合、 **PropertyId**および**propertytag**属性を使用することはできません。<br/><br/>この属性は省略可能です。  <br/> |
|**PropertyId** <br/> |ディスパッチ ID によって拡張プロパティを識別します。 ディスパッチ ID は、10進数または16進数のどちらかの形式で識別できます。 このプロパティは、 **DistinguishedPropertySetId**または**propertysetid**と組み合わせて使用する必要があります。<br/><br/>この属性を使用する場合、 **PropertyName**属性と**propertytag**属性を使用することはできません。<br/><br/>この属性は省略可能です。  <br/> |
|**Recordtype** <br/> |プロパティタグのプロパティの種類を表します。 これは、プロパティタグの重要な単語に対応しています。<br/><br/>このトピックの後半の Recordtype 属性テーブルには、この属性に指定できる値が含まれています。<br/><br/>この属性は必須です。  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>DistinguishedPropertySetId 属性

|**値**|**説明**|
|:-----|:-----|
|アドレス  <br/> |Address プロパティセット ID を名前で識別します。  <br/> |
|Appointment  <br/> |予定のプロパティセット ID を名前で識別します。  <br/> |
|CalendarAssistant  <br/> |カレンダーアシスタントのプロパティセット ID を名前で識別します。  <br/> |
|共通  <br/> |名前によって、共通プロパティセット ID を識別します。  <br/> |
|InternetHeaders  <br/> |インターネットヘッダーのプロパティセット ID を名前で識別します。  <br/> |
|会議  <br/> |名前によって、会議のプロパティセット ID を識別します。  <br/> |
|共有  <br/> | <br/> |
|PublicStrings  <br/> |パブリック文字列のプロパティセット ID を名前で識別します。  <br/> |
|タスク  <br/> |タスクのプロパティセット ID を名前で識別します。  <br/> |
|UnifiedMessaging  <br/> |ユニファイドメッセージングのプロパティセット ID を名前で識別します。  <br/> |
   
#### <a name="propertytype-attribute"></a>Recordtype 属性

|**値**|**説明**|
|:-----|:-----|
|ApplicationTime  <br/> |日付と時刻として解釈される倍精度浮動小数点型 (double) の値を指定します。 整数部分は日付で、小数部分は時刻です。  <br/> |
|ApplicationTimeArray  <br/> |日付と時刻として解釈される倍精度浮動小数点型 (double) の値の配列を指定します。  <br/> |
|バイナリ  <br/> |Base64 でエンコードされたバイナリ値。  <br/> |
|BinaryArray  <br/> |Base64 でエンコードされたバイナリ値の配列。  <br/> |
|ブール型  <br/> |ブール値**true**または**false**。  <br/> |
|CLSID  <br/> |GUID 文字列。  <br/> |
|CLSIDArray  <br/> |GUID 文字列の配列。  <br/> |
|通貨  <br/> |セントの数値として解釈される64ビットの整数。  <br/> |
|CurrencyArray  <br/> |セントの数値として解釈される64ビットの整数の配列。  <br/> |
|倍精度浮動小数点数  <br/> |64ビットの浮動小数点値。  <br/> |
|DoubleArray  <br/> |64ビットの浮動小数点値の配列。  <br/> |
|Error  <br/> |SCODE 値。32ビットの符号なし整数。  <br/> 制限のため、または値の取得および設定には使用されません。 これはレポートにのみ存在します。  <br/> |
|浮動小数点数  <br/> |32ビットの浮動小数点値。  <br/> |
|FloatArray  <br/> |32ビットの浮動小数点値の配列。  <br/> |
|整数  <br/> |符号付き32ビット (Int32) 整数。  <br/> |
|整数配列  <br/> |符号付き32ビット (Int32) 整数の配列。  <br/> |
|Long  <br/> |符号付きまたは符号なしの64ビット (Int64) 整数。  <br/> |
|LongArray  <br/> |符号付きまたは符号なしの64ビット (Int64) 整数の配列。  <br/> |
|Null  <br/> |プロパティ値がないことを示します。  <br/> 制限のため、または値の取得および設定には使用されません。 これはレポートにのみ存在します。  <br/> |
|オブジェクト  <br/> |IUnknown インターフェイスを実装するオブジェクトへのポインター。  <br/> 制限のため、または値の取得および設定には使用されません。 これはレポートにのみ存在します。  <br/> |
|ObjectArray  <br/> |IUnknown インターフェイスを実装するオブジェクトへのポインターの配列。  <br/> 制限のため、または値の取得および設定には使用されません。 これはレポートにのみ存在します。  <br/> |
|長い形式の日付 (スラッシュ区切り)  <br/> |符号付き16ビット整数。  <br/> |
|Short 配列  <br/> |符号付き16ビット整数の配列。  <br/> |
|SystemTime  <br/> |FILETIME 構造体の形式での、64ビットの整数データおよび時刻の値。  <br/> |
|SystemTimeArray  <br/> |FILETIME 構造体の形式で、64ビットの整数データおよび時刻の値の配列。  <br/> |
|文字列  <br/> |Unicode 文字列。  <br/> |
|StringArray  <br/> |Unicode 文字列の配列。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | 追加のプロパティを識別します。<br/><br/>この要素の XPath 式は次のとおりです。<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、アイテムから特定のプロパティを削除するための削除操作を表します。  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |UpdateFolder 呼び出しの実行中にフォルダーから特定のプロパティを削除するための削除操作を表します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを識別します。  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。  <br/> |
|[Exists](exists.md) <br/> |指定されたプロパティがアイテムに存在する場合に**true**を返す検索式を表します。  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |別のプロパティと比較するときに使用するプロパティまたは定数の値を表します。  <br/> |
|[IsEqualTo](isequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、等しい場合は**true**に評価される検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが大きくなる場合は**true**を返す検索式を表します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目のプロパティ以上の場合に**true**を返す検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目のプロパティより小さい場合に**true**を返す検索式を表します。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目のプロパティより小さい場合に**true**を返す検索式を表します。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、値が同じでない場合は**true**を返す検索式を表します。  <br/> |
|[Excludes](excludes.md) <br/> |プロパティのビット単位のマスクを実行します。  <br/> |
|[内容](contains.md) <br/> |指定したプロパティに指定した定数文字列値が含まれているかどうかを決定する検索式を表します。  <br/> |
|[FieldOrder](fieldorder.md) <br/> |結果を並べ替えるための1つのフィールドを表し、並べ替えの方向を示します。  <br/> |
   
## <a name="remarks"></a>注釈

一部の属性は、他の属性と組み合わせて使用することはできません。 拡張プロパティ属性の無効な組み合わせで受け取った要求には、エラーメッセージが生成されます。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
> [!NOTE]
> Microsoft .NET では、Long は64ビットの符号付き整数です。 MAPI と COM では、Long は32ビットの整数です。 ほとんどの開発者は、Microsoft.NET フレームワークを使用して、Exchange Web サービスクライアントアプリケーションを開発します。 そのため、MAPI の名前付けの代わりに .NET の名前付けを使用します。
> 
> たとえば、PR_MESSAGE_FLAGS MAPI プロパティ0x0E07 は、PT \_ LONG 型です。 .NET では、これは整数と見なされます。 PR_MESSAGE_FLAGS の拡張プロパティは、として定義され `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>` ます。 
  
## <a name="example"></a>例

次の要求例では、2つのカスタムプロパティを持つアイテムを作成します。 最初のカスタムプロパティは、ブール値が**true**に設定された**ismyhouse**という名前です。 2番目のカスタム拡張プロパティには、 **HousePrices**という名前が付けられます。 通貨値の配列が含まれています。 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

