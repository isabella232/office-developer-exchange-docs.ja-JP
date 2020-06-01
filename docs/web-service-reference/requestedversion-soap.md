---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: RequestedVersion 要素は、クライアントが要求を処理する必要のある最小サービスバージョンを指定します。
ms.openlocfilehash: ded276b3eb2c70b6edd39ca12289098de2b3faea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459168"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

**Requestedversion**要素は、クライアントが要求を処理する必要のある最小サービスバージョンを指定します。 
  
```XML
<RequestedVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[要求 (SOAP)](request-soap.md) <br/> |要求された構成設定と対象ユーザーが含まれます。  <br/> |
|[Request (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |ドメイン設定を取得するための要求を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Requestedversion**要素のテキスト値には、Exchange2010、Exchange2010_SP1、Exchange2010_SP2、または Exchange2013 を指定できます。
  
## <a name="remarks"></a>注釈

この要素が存在しない場合は、最新のサービスバージョンが使用されます。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

