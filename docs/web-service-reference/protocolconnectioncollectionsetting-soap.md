---
title: ProtocolConnectionCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 51f84364-9a5f-4ef2-ba82-f6ef7c65f7cb
description: ProtocolConnectionCollectionSetting 要素は、サーバー プロトコルの接続の設定のコレクションを表します。
ms.openlocfilehash: d0342222c0390d3e49afe572af92a903b9643a2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832914"
---
# <a name="protocolconnectioncollectionsetting-soap"></a>ProtocolConnectionCollectionSetting (SOAP)

**ProtocolConnectionCollectionSetting**要素は、サーバー プロトコルの接続の設定のコレクションを表します。 
  
```XML
<ProtocolConnectionCollectionSetting/>
   <Name/>
   <ProtocolConnections/>
</ProtocolConnectionCollectionSetting>
```

 **ProtocolConnectionCollectionSetting**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[名 (SOAP)](name-soap.md) <br/> |設定の名前を表します。  <br/> |
|[ProtocolConnections (SOAP)](protocolconnections-soap.md) <br/> |0 個以上のプロトコルの接続が含まれています。  <br/> |
   
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
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
  
[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)

