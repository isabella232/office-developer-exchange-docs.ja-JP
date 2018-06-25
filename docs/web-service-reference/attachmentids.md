---
title: AttachmentIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentIds
api_type:
- schema
ms.assetid: 46ce3ad7-4b20-43ae-8c63-39f1e3c2666b
description: AttachmentIds 要素には、添付ファイルの識別子の配列が含まれています。
ms.openlocfilehash: f205aefe6a7dc4ec208e8a96b8a6b47094aa741b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759454"
---
# <a name="attachmentids"></a>AttachmentIds

**AttachmentIds**要素には、添付ファイルの識別子の配列が含まれています。 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 **NonEmptyArrayOfRequestAttachmentIdsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AttachmentId (GetAttachment と DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) <br/> |単一の添付ファイルを識別する要素です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DeleteAttachment](deleteattachment.md) <br/> |Exchange ストアからの添付ファイルを削除する要求を定義する要素。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/DeleteAttachment` <br/> |
|[GetAttachment](getattachment.md) <br/> |Exchange ストアからの添付ファイルを取得する要求を定義する要素。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteAttachment 操作](deleteattachment-operation.md)
- [GetAttachment 操作](getattachment-operation.md)

