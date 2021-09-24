---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: ParentItemId 要素は、関連付けられた添付ファイルにリンクする親アイテムを識別します。
ms.openlocfilehash: d8072e86d8bd989d4baf6b0f29385dc955b83de8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515363"
---
# <a name="parentitemid"></a>ParentItemId

**ParentItemId 要素は**、関連付けられた添付ファイルにリンクする親アイテムを識別します。 
  
- [CreateAttachment](createattachment.md)
  
- [ParentItemId](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**ItemIdType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |添付ファイルに関連付けるExchangeストア内の 1 つのアイテムを識別します。 この値は文字列です。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |Id 属性によって識別されるアイテムの指定されていないバージョンを、Exchangeします。  これは、添付ファイルを更新するときに現在のアイテムが使用されるのを確認するために使用されます。 この値は文字列です。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |メールボックス内のアイテムへの添付ファイルを作成する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>注釈

この要素は [、CreateAttachment 操作で必要です](createattachment-operation.md)。 この要素は基本的に [ItemId 要素と同](itemid.md) じです。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [CreateAttachment 操作](createattachment-operation.md)

