---
title: User (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: User 要素は、1 人のユーザーの ID を表します。
ms.openlocfilehash: 545869e21726d60ecdd503106c743d66fc752414
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517379"
---
# <a name="user-soap"></a>User (SOAP)

**User 要素** は、1 人のユーザーの ID を表します。 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 **ユーザー**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |代替メールボックスの従来の識別名を表します。  <br/> |
|[Mailbox (SOAP)](mailbox-soap.md) <br/> |検出するユーザーの電子メール アドレスが含まれる。  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |要求された構成設定の名前が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー (SOAP)](users-soap.md) <br/> |User 要素のコレクション **を表** します。  <br/> |
   
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
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
  
[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

