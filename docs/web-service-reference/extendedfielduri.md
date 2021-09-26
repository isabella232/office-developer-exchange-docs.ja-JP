---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: ExtendedFieldURI 要素は、拡張 MAPI プロパティを識別します。
ms.openlocfilehash: 0cf3926c900e1b1f35018c6706cfe99ebefbe76f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542317"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

**ExtendedFieldURI 要素** は、拡張 MAPI プロパティを識別します。 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |拡張 MAPI プロパティの既知のプロパティ セットの ID を定義します。<br/><br/>この属性を使用すると **、PropertySetId** 属性と **PropertyTag** 属性を使用できません。 この属性は **、PropertyId** 属性または PropertyName 属性、 **および PropertyType** 属性と一緒に **使用する必要** があります。<br/><br/>この **トピックの後半にある DistinguishedPropertySetId** 属性テーブルには、この属性に使用できる値の一覧が示されています。<br/><br/>この属性は省略可能です。  <br/> |
|**PropertySetId** <br/> |MAPI 拡張プロパティ セットまたは名前空間を識別する GUID によって識別します。<br/><br/>この属性を使用する場合は **、DistinguishedPropertySetId** 属性と **PropertyTag** 属性を使用できません。 この属性は **、PropertyId** 属性または PropertyName 属性、 **および PropertyType** 属性と一緒に **使用する必要** があります。<br/><br/>この属性は省略可能です。  <br/> |
|**PropertyTag** <br/> |タグの型部分のないプロパティ タグを識別します。 **PropertyTag は**、16 進数または短整数として表されます。<br/><br/>プロパティとプロパティ0x8000 0xFFFEプロパティのカスタム範囲を表します。 メールボックス データベースが初めてカスタム プロパティを検出すると、そのカスタム プロパティに、カスタム プロパティの範囲内の 0x8000-0xFFFE のプロパティ タグが割り当0xFFFE。 特定のカスタム プロパティ タグは、ほとんどの場合、データベース間で異なります。 したがって、プロパティ タグによるカスタム プロパティ要求は、データベースごとに異なるプロパティを返す可能性があります。 PropertyTag 属性 **の使用** は、カスタム プロパティでは禁止されています。 代わりに **、PropertySetId** 属性と **PropertyName** 属性または **PropertyId 属性を使用** します。<br/><br/>**重要**: GUID + 名前/ID を使用して0x8000と0xFFFEのカスタム プロパティにアクセスします。 **PropertyTag 属性を** 使用する場合は **、DistinguishedPropertySetId、PropertySetId、PropertyName、****および PropertyId** 属性を使用できません。  <br/><br/>この属性は省略可能です。<br/><br/>**注**: カスタム範囲内のプロパティにプロパティ タグ属性を使用0x8000-0xFFFE。 この場合は、名前付きプロパティを使用する必要があります。           |
|**PropertyName** <br/> |拡張プロパティを名前で識別します。 このプロパティは **、DistinguishedPropertySetId** または **PropertySetId と結合する必要があります**。<br/><br/>この属性を使用する場合は **、PropertyId** 属性と **PropertyTag** 属性を使用できません。<br/><br/>この属性は省略可能です。  <br/> |
|**PropertyId** <br/> |拡張プロパティをディスパッチ ID で識別します。 ディスパッチ ID は、10 進数または 16 進形式で識別できます。 このプロパティは **、DistinguishedPropertySetId** または **PropertySetId と結合する必要があります**。<br/><br/>この属性を使用すると **、PropertyName** 属性と **PropertyTag** 属性を使用できません。<br/><br/>この属性は省略可能です。  <br/> |
|**PropertyType** <br/> |プロパティ タグのプロパティの種類を表します。 これは、プロパティ タグ内の最も重要な単語に対応します。<br/><br/>このトピックの後の PropertyType 属性テーブルには、この属性に使用できる値が含まれます。<br/><br/>この属性は必須です。  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>DistinguishedPropertySetId 属性

|**値**|**説明**|
|:-----|:-----|
|アドレス  <br/> |アドレス プロパティ セット ID を名前で識別します。  <br/> |
|Appointment  <br/> |予定プロパティ セット ID を名前で識別します。  <br/> |
|CalendarAssistant  <br/> |予定表アシスタント プロパティ セット ID を名前で識別します。  <br/> |
|共通  <br/> |共通プロパティ セット ID を名前で識別します。  <br/> |
|InternetHeaders  <br/> |インターネット ヘッダー プロパティ セット ID を名前で識別します。  <br/> |
|会議  <br/> |会議プロパティ セット ID を名前で識別します。  <br/> |
|共有  <br/> | <br/> |
|PublicStrings  <br/> |パブリック文字列プロパティ セット ID を名前で識別します。  <br/> |
|タスク  <br/> |タスク プロパティ セット ID を名前で識別します。  <br/> |
|UnifiedMessaging  <br/> |名前でユニファイド メッセージング プロパティ セット ID を識別します。  <br/> |
   
#### <a name="propertytype-attribute"></a>PropertyType 属性

|**値**|**説明**|
|:-----|:-----|
|ApplicationTime  <br/> |日付と時刻として解釈される倍数の値。 整数部分は日付で、分数部分は時刻です。  <br/> |
|ApplicationTimeArray  <br/> |日付と時刻として解釈される倍数の値の配列。  <br/> |
|Binary  <br/> |Base64 でエンコードされたバイナリ値。  <br/> |
|BinaryArray  <br/> |Base64 でエンコードされたバイナリ値の配列。  <br/> |
|ブール型  <br/> |ブール型 **(True) または** **false です**。  <br/> |
|CLSID  <br/> |GUID 文字列。  <br/> |
|CLSIDArray  <br/> |GUID 文字列の配列。  <br/> |
|通貨  <br/> |セント数として解釈される 64 ビット整数。  <br/> |
|CurrencyArray  <br/> |セント数として解釈される 64 ビット整数の配列。  <br/> |
|Double  <br/> |64 ビット浮動小数点値。  <br/> |
|DoubleArray  <br/> |64 ビット浮動小数点値の配列。  <br/> |
|Error  <br/> |SCODE 値。32 ビット符号なし整数。  <br/> 制限や値の取得/設定には使用されません。 これはレポート用にのみ存在します。  <br/> |
|浮動小数点数  <br/> |32 ビット浮動小数点値。  <br/> |
|FloatArray  <br/> |32 ビット浮動小数点値の配列。  <br/> |
|整数  <br/> |符号付き 32 ビット (Int32) 整数。  <br/> |
|IntegerArray  <br/> |符号付き 32 ビット (Int32) 整数の配列。  <br/> |
|Long  <br/> |符号付きまたは符号なし 64 ビット (Int64) の整数。  <br/> |
|LongArray  <br/> |符号付きまたは符号なし 64 ビット (Int64) 整数の配列。  <br/> |
|Null  <br/> |プロパティ値なしを示します。  <br/> 制限や値の取得/設定には使用されません。 これはレポート用にのみ存在します。  <br/> |
|オブジェクト  <br/> |IUnknown インターフェイスを実装するオブジェクトへのポインター。  <br/> 制限や値の取得/設定には使用されません。 これはレポート用にのみ存在します。  <br/> |
|ObjectArray  <br/> |IUnknown インターフェイスを実装するオブジェクトへのポインターの配列。  <br/> 制限や値の取得/設定には使用されません。 これはレポート用にのみ存在します。  <br/> |
|長い形式の日付 (スラッシュ区切り)  <br/> |符号付き 16 ビット整数。  <br/> |
|ShortArray  <br/> |符号付き 16 ビット整数の配列。  <br/> |
|SystemTime  <br/> |FILETIME 構造体の形式の 64 ビット整数データと時刻値。  <br/> |
|SystemTimeArray  <br/> |FILETIME 構造体の形式の 64 ビット整数データと時刻値の配列。  <br/> |
|String  <br/> |Unicode 文字列。  <br/> |
|StringArray  <br/> |Unicode 文字列の配列。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | 追加のプロパティを識別します。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |UpdateItem 操作内のアイテムの 1 つのプロパティへの更新 [を表します](updateitem-operation.md)。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |UpdateFolder 操作のフォルダー上の 1 つのプロパティへの更新 [を表します](updatefolder-operation.md)。  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |UpdateItem 操作中にアイテムから特定のプロパティを削除するための削除操作 [を表します](updateitem-operation.md)。  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |UpdateFolder 呼び出し中にフォルダーから特定のプロパティを削除するための削除操作を表します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |UpdateItem 操作中にアイテムの 1 つのプロパティに追加する [データを識別します](updateitem-operation.md)。  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |UpdateFolder 操作中にフォルダー プロパティに追加する [データを指定します](updatefolder-operation.md)。  <br/> |
|[Exists](exists.md) <br/> |指定されたプロパティがアイテムに存在する場合に **true** を返す検索式を表します。  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |別のプロパティと比較するときに使用するプロパティまたは定数値を表します。  <br/> |
|[IsEqualTo](isequalto.md) <br/> |プロパティと定数値または別のプロパティを比較し、等しい場合は **true** と評価される検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |プロパティを定数値または別のプロパティと比較する検索式を表し、最初のプロパティが大きい場合は **true** を返します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが 2 番目のプロパティ以上の場合は **true** を返す検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが 2 番目のプロパティより小さい場合は **true** を返す検索式を表します。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが 2 番目のプロパティより小さい場合は **true** を返す検索式を表します。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |定数値または別のプロパティとプロパティを比較する検索式を表し、値が同じではない場合は **true** を返します。  <br/> |
|[Excludes](excludes.md) <br/> |プロパティのビットのマスクを実行します。  <br/> |
|[Contains](contains.md) <br/> |指定したプロパティに指定された定数文字列値が含まれているかどうかを決定する検索式を表します。  <br/> |
|[FieldOrder](fieldorder.md) <br/> |結果を並べ替える 1 つのフィールドを表し、並べ替えの方向を示します。  <br/> |
   
## <a name="remarks"></a>注釈

一部の属性は、他の属性と組み合わせて使用できません。 拡張プロパティ属性の無効な組み合わせが含まれている要求は、エラー メッセージを生成します。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
> [!NOTE]
> Microsoft .NET では、Long は 64 ビットの符号付き整数で、MAPI と COM では Long は 32 ビット整数です。 ほとんどの開発者は、Microsoft.NET フレームワークを使用して、Web Services Exchangeアプリケーションを開発します。 したがって、.NET 名前付けは MAPI の名前付けではなく使用されます。
> 
> たとえば、MAPI プロパティPR_MESSAGE_FLAGSは、0x0E07 PT LONG 型 \_ です。 .NET では、これは整数と見なされます。 プロパティの拡張プロパティは、PR_MESSAGE_FLAGSとして定義されます `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>` 。 
  
## <a name="example"></a>例

次の要求の例では、2 つのカスタム プロパティを持つアイテムを作成します。 最初のカスタム プロパティは **IsMyHouse という名前で、** ブール値は true に設定 **されています**。 2 番目のカスタム拡張プロパティは **、HousePrices という名前です**。 通貨の値の配列が含まれます。 
  
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
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

