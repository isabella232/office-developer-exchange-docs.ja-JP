---
title: base64FolderId (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: base64FolderId 要素には、SetTelephoneAccessFolderEmail 操作 (UM Web サービス) 要求でユニファイド メッセージングが電話でメッセージを読み取る既定の電子メール フォルダーとして指定するフォルダーの識別子が含まれます。
ms.openlocfilehash: 149ad55d0ab09f57b0dc3ace7eb0e17c96265e3f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518933"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (UM Web サービス)

**base64FolderId** 要素には [、SetTelephoneAccessFolderEmail 操作 (UM Web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)要求でユニファイド メッセージングが電話でメッセージを読み取る既定の電子メール フォルダーとして指定するフォルダーの識別子が含まれます。 
  
[SetTelephoneAccessFolderEmail (UM Web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (UM Web サービス)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (UM Web サービス)](settelephoneaccessfolderemail-um-web-service.md) <br/> |電話アクセス電子メール フォルダーを設定する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、フォルダーの MAPI ID を表します。
  
## <a name="remarks"></a>注釈

電話アクセス電子メール フォルダーを設定するには [、SetTelephoneAccessFolderEmail 操作 (UM Web サービス) を使用します](settelephoneaccessfolderemail-operation-um-web-service.md)。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SetTelephoneAccessFolderEmail (UM Web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmail 操作 (UM Web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[FindFolder 操作](findfolder-operation.md)
  
[FindItem 操作](finditem-operation.md)

