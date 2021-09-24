---
title: ユーザー (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: Users 要素は、設定を取得する必要があるユーザーの電子メール アドレスのコレクションを表します。
ms.openlocfilehash: eabf0d2cd38396e907ca467596c2e55d1eb78e02
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538521"
---
# <a name="users-soap"></a>ユーザー (SOAP)

**Users 要素** は、設定を取得する必要があるユーザーの電子メール アドレスのコレクションを表します。 
  
```XML
<Users>
   <User/>
</Users>
```

 **Users**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[User (SOAP)](user-soap.md) <br/> |ユーザーの電子メール アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |1 人または複数のユーザーの指定した設定を取得する要求を表します。  <br/> |
|[Request (SOAP)](request-soap.md) <br/> |要求された構成設定とターゲット ユーザーが含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

