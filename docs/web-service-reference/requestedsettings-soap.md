---
title: RequestedSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: RequestedSettings 要素には、要求された構成設定の名前が含まれています。
ms.openlocfilehash: 025f86d417ea2041a3247ac67b065d75c8f75599
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833136"
---
# <a name="requestedsettings-soap"></a>RequestedSettings (SOAP)

**RequestedSettings**要素には、要求された構成設定の名前が含まれています。 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 **RequestedSettings**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[(SOAP) の設定](setting-soap.md) <br/> |返される構成設定を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |1 つまたは複数のユーザーに対して指定した設定を取得する要求を表します。  <br/> |
|[要求 (SOAP)](request-soap.md) <br/> |要求された構成設定とユーザーを対象に含まれています。  <br/> |
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。  <br/> |
   
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

