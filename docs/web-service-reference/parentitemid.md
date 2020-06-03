---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: ParentItemId 要素は、関連付けられた添付ファイルにリンクする親アイテムを識別します。
ms.openlocfilehash: 4f3e33da0af2438948313f0e335cd03e076d135a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465745"
---
# <a name="parentitemid"></a>ParentItemId

**Parentitemid**要素は、関連付けられた添付ファイルにリンクする親アイテムを識別します。 
  
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
|**Id** <br/> |添付ファイルに関連付ける Exchange ストア内の1つのアイテムを識別します。 この値は文字列です。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |Exchange ストアの**Id**属性によって識別されるアイテムの指定されていないバージョンを識別します。 これは、添付ファイルによって更新されるときに、現在のアイテムが使用されるようにするために使用されます。 この値は文字列です。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |メールボックス内のアイテムの添付ファイルを作成するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>注釈

この要素は、 [Createattachment 操作](createattachment-operation.md)で必要です。 この要素は、基本的に[ItemId](itemid.md)要素と同じです。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [CreateAttachment 操作](createattachment-operation.md)

