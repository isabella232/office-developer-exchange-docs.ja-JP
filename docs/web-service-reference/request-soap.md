---
title: 要求 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: 要求要素には、要求された構成設定と対象ユーザーが含まれています。
ms.openlocfilehash: 4358713d19e763b75d2a43f147385026f43b1255
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448990"
---
# <a name="request-soap"></a>要求 (SOAP)

**要求**要素には、要求された構成設定と対象ユーザーが含まれています。 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 **GetUserSettingsRequest**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Users (SOAP)](users-soap.md) <br/> |設定を取得するユーザーの電子メールアドレスのコレクションを表します。  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |要求された構成設定の名前が含まれています。  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |プロバイダーが使用する特定のサーバーのバージョンを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserSettingsRequestMessage (SOAP)](getusersettingsrequestmessage-soap.md) <br/> |[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

