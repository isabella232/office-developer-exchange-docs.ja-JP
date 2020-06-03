---
title: base64FolderId (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: Base64FolderId 要素には、ユニファイドメッセージングが SetTelephoneAccessFolderEmail 操作 (UM web サービス) 要求で電話でメッセージを読み取る既定の電子メールフォルダーとして指定するフォルダーの識別子が含まれています。
ms.openlocfilehash: ea31c7a0f93188e563bf95c4a3e6e91f0866746c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458048"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (UM web サービス)

**Base64FolderId**要素には、ユニファイドメッセージングが[SETTELEPHONEACCESSFOLDEREMAIL 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)要求で電話でメッセージを読み取る既定の電子メールフォルダーとして指定するフォルダーの識別子が含まれています。 
  
[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (UM web サービス)](base64folderid-um-web-service.md)
  
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
|[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md) <br/> |電話アクセスの電子メールフォルダーを設定するための要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 Text 値は、フォルダーの MAPI ID を表します。
  
## <a name="remarks"></a>注釈

電話アクセスの電子メールフォルダーを設定するには、 [SetTelephoneAccessFolderEmail 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)を使用します。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmail 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[FindFolder 操作](findfolder-operation.md)
  
[FindItem 操作](finditem-operation.md)

