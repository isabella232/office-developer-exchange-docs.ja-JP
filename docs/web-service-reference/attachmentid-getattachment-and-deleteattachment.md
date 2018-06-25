---
title: AttachmentId (GetAttachment と DeleteAttachment)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 4bea1cb5-0a0f-4e14-9b09-f91af8cf9899
description: AttachmentId 要素は、単一の添付ファイルを識別します。
ms.openlocfilehash: b0355b4a387c65e97fe973a1667e6b0a517ebf7e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759453"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a>AttachmentId (GetAttachment と DeleteAttachment)

**AttachmentId**要素は、単一の添付ファイルを識別します。 
  
```xml
<AttachmentId Id="" />
```

 **RequestAttachmentIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |添付ファイル識別子を指定します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AttachmentIds](attachmentids.md) <br/> | 添付ファイル識別子の配列が含まれています。<br/><br/>  この要素への XPath 式は、次のように。<br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [DeleteAttachment 操作](deleteattachment-operation.md)
- [GetAttachment 操作](getattachment-operation.md)

