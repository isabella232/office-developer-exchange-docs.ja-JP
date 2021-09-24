---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: ContactsView 要素は、アルファベット順の表示名に基づいて連絡先アイテムの検索を定義します。
ms.openlocfilehash: a96da6270d2396e5e82851dcc200f818cec5a7ed
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531100"
---
# <a name="contactsview"></a>ContactsView

**ContactsView 要素は**、アルファベット順の表示名に基づいて連絡先アイテムの検索を定義します。 
  
[FindItem](finditem.md)
  
[ContactsView](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

**ContactsViewType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |FindItem 応答で返される結果の最大数 [を示](finditem.md) します。  <br/> |
|**InitialName** <br/> |応答で返す連絡先リストの最初の名前を定義します。 指定された初期名が連絡先リストに含されていない場合、次の名前が FinalName の後に付く場合を除き、文化コンテキストで定義されている次のアルファベット名 **が返されます**。 **InitialName 属性を** 省略すると、応答には連絡先リストの最初の名前で始まる連絡先の一覧が含まれる。 この属性は省略可能です。  <br/> |
|**FinalName** <br/> |応答で返す連絡先リストの最後の名前を定義します。 **FinalName 属性を** 省略すると、応答には後続のすべての連絡先が指定した並べ替え順序で含まれる。 指定した最終名が連絡先リストに含めされていない場合、文化コンテキストで定義されている次のアルファベットの名前は除外されます。  <br/><br/>たとえば、FinalName="Name" が連絡先リストに含まれていない場合、Name1 または NAME の表示名を持つ連絡先は含まれません。  <br/><br/>この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。<br/><br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の要求の例は、Kelly Rollin という表示名を持つ連絡先から始まる最初の 3 つの連絡先を検索する方法を示しています。
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
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

- [FindItem 操作](finditem-operation.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

