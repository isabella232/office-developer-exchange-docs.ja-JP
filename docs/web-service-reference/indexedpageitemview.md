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
description: IndexedPageItemView 要素は、ページがどのように会話を説明または FindItem 操作または FindConversation 操作の要求の情報が返される項目です。
ms.openlocfilehash: f1743e22087158c1889977f03774fccbc5577390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831919"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

**IndexedPageItemView**要素は、ページがどのように会話を説明または[FindItem 操作](finditem-operation.md)または[FindConversation 操作](findconversation-operation.md)の要求の情報が返される項目です。 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |アイテムや会話の応答を返すの最大数について説明します。 この属性は、省略可能です。  <br/> |
|**Offset** <br/> |**ベース ポイント**からのオフセットを示します。 **ベース ポイント**と等しい場合、開始オフセットが正の数値です。 **ベース ポイント**が終了する場合、オフセットが負の場合と処理されます。 どの項目を識別または会話の応答で配信される最初になります。 この属性は、必要があります。  <br/> |
|**ベース ポイント** <br/> |項目やテーマのページを一連の項目または検索条件を使用して検出された会話の前後から開始されるかどうかについて説明します。 末尾からのシークを常に検索を進めます。 この属性は、必要があります。  <br/> |
   
#### <a name="basepoint-attribute"></a>ベース ポイントの属性

|**値**|**説明**|
|:-----|:-----|
|先頭  <br/> |ページ ビューでは、会話やアイテムの検索結果セットの先頭から開始されます。  <br/> |
|終了  <br/> |ページ ビューは、見つかった会話やアイテム セットの末尾から開始します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内の会話を検索するための要求を定義します。  <br/> |
   
## <a name="remarks"></a>備考

末尾からのシークでは、オフセットによって識別される原点に移動します。 さらに、ポインターが再び要求されたレコードの数によって。 などの場合は 100 個のレコードがある、オフセットが末尾から 25、75 から検索を開始します。 10 個のレコードが返された場合ポインターが逆方向、さらに 10 が 65 を記録し、65 75 からのレコードを返します。 次のインデックスは、64 です。 ページの末尾からの次のオフセットは、100-36 に相当する 64 です。 36 は、次のインデックス付きのページを取得する、末尾からの次のオフセットの値です。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

[FindItem 操作](finditem-operation.md)要求の例を次に示します。 ID とトピックは、各項目が返されます。 最大六つのアイテムは、 **MaxEntriesReturned**属性で指定されている、応答で返されます。 アイテムは、重要度別にグループ化の順序を昇順に表示されます。 グループ内のアイテムは、件名ごとに集約されます。 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindItem 操作](finditem-operation.md)
  

  [FindConversation 操作](findconversation-operation.md)


[項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

