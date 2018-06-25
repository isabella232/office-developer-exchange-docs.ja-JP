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
description: ParentItemId 要素は、関連付けられている添付ファイルへのリンクを親項目を識別します。
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832703"
---
# <a name="parentitemid"></a>ParentItemId

**ParentItemId**要素は、関連付けられている添付ファイルへのリンクを親項目を識別します。 
  
- [CreateAttachment](createattachment.md)
  
- [ParentItemId](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**ItemIdType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |添付ファイルを関連付けるには Exchange ストア内の 1 つの項目を識別します。 この値は、文字列です。 この属性は、必要があります。  <br/> |
|**変更キー** <br/> |Exchange ストア内の**Id**属性によって識別される項目の指定のバージョンを識別します。 これを使用して、添付ファイルを更新するときに現在の項目が使用されているかどうかを確認します。 この値は、文字列です。 この属性は、省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |メールボックス内のアイテムに添付ファイルを作成する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>備考

[CreateAttachment 操作](createattachment-operation.md)では、この要素が必要です。 この要素は、基本的に[アイテム Id](itemid.md)の要素と同じです。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [CreateAttachment 操作](createattachment-operation.md)

