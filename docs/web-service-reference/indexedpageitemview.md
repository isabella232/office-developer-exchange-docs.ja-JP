---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: IndexedPageItemView 要素は、FindItem 操作または FindConversation 操作要求に対して、ページ会話またはアイテム情報がどのように返されるのかについて説明します。
ms.openlocfilehash: bf46bdbd457c4f4fa47e6b575d3b797b74f58995
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541127"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

**IndexedPageItemView** 要素は [、FindItem](finditem-operation.md)操作または [FindConversation](findconversation-operation.md)操作要求に対して、ページ会話またはアイテム情報がどのように返されるのかについて説明します。 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |応答で返されるアイテムまたは会話の最大数を示します。 この属性は省略可能です。  <br/> |
|**Offset** <br/> |BasePoint からのオフセットについて **説明します**。 **BasePoint が Beginning** に等しい場合、オフセットは正の値です。 **BasePoint が End** に等しい場合、オフセットは負の値である場合と同様に処理されます。 これは、応答で配信される最初のアイテムまたは会話を識別します。 この属性は必須です。  <br/> |
|**BasePoint** <br/> |アイテムまたは会話のページが、検索条件を使用して見つかった一連のアイテムまたは会話の先頭または末尾から開始するかどうかを示します。 最後からシークすると、常に後方に検索されます。 この属性は必須です。  <br/> |
   
#### <a name="basepoint-attribute"></a>BasePoint 属性

|**値**|**説明**|
|:-----|:-----|
|開始  <br/> |ページ ビューは、見つかった会話またはアイテム セットの先頭から始まります。  <br/> |
|End  <br/> |ページ ビューは、見つかった会話またはアイテム セットの最後から開始します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内の会話を検索する要求を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

最後からシークするには、オフセットで識別される原点に移動します。 さらに、ポインターは要求されたレコードの数によって戻されます。 たとえば、レコードが 100 件で、オフセットが末尾から 25 の場合、検索は 75 から始まります。 10 レコードが返された場合、ポインターは追加の 10 レコードを 65 に戻し、レコード 65 から 75 を返します。 次のインデックスは 64 です。 ページの末尾からの次のオフセットは 100 ~ 64 で、36 に等しくなります。 36 は、次のインデックス付きページを取得する最後からの次のオフセットの値です。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例は [、FindItem 操作要求を示](finditem-operation.md) しています。 各アイテムは ID と件名で返されます。 **MaxEntriesReturned** 属性で指定された最大 6 つのアイテムが応答で返されます。 アイテムは、重要度でグループ化された昇順で一覧表示されます。 グループ内のアイテムは件名別に集計されます。 
  
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
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)
  
[FindConversation 操作](findconversation-operation.md)


[アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

