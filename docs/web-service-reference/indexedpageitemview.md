---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: IndexedPageItemView 要素は、ページ化された会話またはアイテム情報が FindItem 操作または FindConversation 操作要求に対してどのように返されるかを表します。
ms.openlocfilehash: 0a66f17855fd425082e3651886d3eeec4f217ac4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456914"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

**Indexedpageitemview**要素は、ページ化された会話またはアイテム情報が[FindItem 操作](finditem-operation.md)または[findconversation 操作](findconversation-operation.md)要求に対してどのように返されるかを表します。 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |応答で返されるアイテムまたはスレッドの最大数を表します。 この属性は省略可能です。  <br/> |
|**Offset** <br/> |**BasePoint**からのオフセットを記述します。 **BasePoint**が先頭と等しい場合、オフセットは正になります。 **BasePoint**が End と等しい場合、オフセットは負の値として処理されます。 これにより、応答で最初に配信されるアイテムまたは会話が特定されます。 この属性は必須です。  <br/> |
|**BasePoint** <br/> |アイテムまたはスレッドのページが、検索条件を使用して検出されたアイテムまたは会話のセットの先頭または末尾から開始するかどうかを指定します。 末尾からシークすると、常に逆方向に検索されます。 この属性は必須です。  <br/> |
   
#### <a name="basepoint-attribute"></a>BasePoint 属性

|**値**|**説明**|
|:-----|:-----|
|始まる  <br/> |ページビューは、検出されたスレッドまたはアイテムセットの先頭から開始されます。  <br/> |
|End  <br/> |ページビューは、検出されたスレッドまたはアイテムセットの末尾から開始されます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内のスレッドを検索する要求を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

最後からシークするには、オフセットで識別される原点への移動が必要になります。 さらに、要求されたレコードの数だけポインターが戻されます。 たとえば、100レコードがあり、オフセットが最後から25である場合、検索は75から開始されます。 10件のレコードが返された場合、ポインターは10レコード後ろに65に移動され、レコード 65 ~ 75 を返します。 次のインデックスは64です。 ページの最後からの次のオフセットは、36と等しい 100-64 です。 36は、次のインデックスページを取得するために末尾からの次のオフセットの値です。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例は、 [FindItem 操作](finditem-operation.md)要求を示しています。 各アイテムは、ID と subject で返されます。 応答では、 **maxん返さ**れた属性によって指定されているように、最大6つのアイテムが返されます。 アイテムは重要度別にグループ化されて昇順に表示されます。 グループ内のアイテムは、件名によって集約されます。 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <IndexedPageItemView MaxEntriesReturned="6" BasePoint="Beginning" Offset="0" />
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)
  
[FindConversation 操作](findconversation-operation.md)


[アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

