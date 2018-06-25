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
description: 要求要素には、要求された構成設定とターゲットのユーザーが含まれています。
ms.openlocfilehash: dfea33786066dd7803d0fd061cbb87bb06d11531
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833125"
---
# <a name="request-soap"></a>要求 (SOAP)

**要求**の要素には、要求された構成設定とターゲットのユーザーが含まれています。 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 **GetUserSettingsRequest**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー (SOAP)](users-soap.md) <br/> |設定を取得する対象となるユーザーの電子メール アドレスのコレクションを表します。  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |要求された構成設定の名前が含まれています。  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |プロバイダーの利用を希望する特定のサーバーのバージョンを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserSettingsRequestMessage (SOAP)](getusersettingsrequestmessage-soap.md) <br/> |[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

