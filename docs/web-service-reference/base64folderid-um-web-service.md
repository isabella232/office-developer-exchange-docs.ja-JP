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
description: Base64FolderId 要素には、元となるユニファイド メッセージング メッセージを読み取り、SetTelephoneAccessFolderEmail の操作 (UM web サービス) の要求に電話で、既定の電子メール フォルダーとして指定するフォルダーの識別子が含まれています。
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759488"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (UM web サービス)

**Base64FolderId**要素には、元となるユニファイド メッセージング メッセージを読み取り[(UM web サービス) の SetTelephoneAccessFolderEmail 操作](settelephoneaccessfolderemail-operation-um-web-service.md)の要求の電話で、既定の電子メール フォルダーとして指定するフォルダーの識別子が含まれています。 
  
[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (UM web サービス)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md) <br/> |電子メール フォルダーには、電話のアクセスを設定する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、フォルダーの MAPI ID を表します。
  
## <a name="remarks"></a>備考

電子メール フォルダーには、電話のアクセスを設定するには、 [SetTelephoneAccessFolderEmail 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)を使用します。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmail 操作 (UM web サービス)](settelephoneaccessfolderemail-operation-um-web-service.md)
  

  [FindFolder 操作](findfolder-operation.md)
  

  [FindItem 操作](finditem-operation.md)

