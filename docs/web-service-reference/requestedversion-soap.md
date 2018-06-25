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
description: RequestedVersion 要素は、クライアントが要求の処理を依頼する最低限のサービスのバージョンを指定します。
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833134"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

**RequestedVersion**要素は、クライアントが要求の処理を依頼する最低限のサービスのバージョンを指定します。 
  
```XML
<RequestedVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[要求 (SOAP)](request-soap.md) <br/> |要求された構成設定とユーザーを対象に含まれています。  <br/> |
|[要求 (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |ドメインの設定を取得する要求を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**RequestedVersion**要素のテキスト値には、Exchange2010、Exchange2010_SP1、Exchange2010_SP2、または Exchange2013 を指定できます。
  
## <a name="remarks"></a>備考

この要素が存在しない場合は、サービスの最新バージョンが使用されます。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

