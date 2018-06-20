---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: GetUserSettingsRequest 要素は、1 つまたは複数のユーザーに対して指定した設定を取得する要求を表します。
ms.openlocfilehash: dc22570144a6947dc6e7042326c7416422680cc1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831702"
---
# <a name="getusersettingsrequest-soap"></a>GetUserSettingsRequest (SOAP)

**GetUserSettingsRequest**要素は、1 つまたは複数のユーザーに対して指定した設定を取得する要求を表します。 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
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

なし。
  
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

