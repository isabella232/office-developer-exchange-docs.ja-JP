---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: RequestVersion 要素は、クライアントが要求を処理する最小サービス バージョンを指定します。
ms.openlocfilehash: 390dee362bf2e6c2bdeac4e0e5564ecbd59b7319
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513333"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

**RequestVersion** 要素は、クライアントが要求を処理する最小サービス バージョンを指定します。 
  
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
|[Request (SOAP)](request-soap.md) <br/> |要求された構成設定とターゲット ユーザーが含まれる。  <br/> |
|[Request (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |ドメイン設定を取得する要求を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

RequestedVersion 要素の **テキスト値** は、Exchange2010、Exchange2010_SP1、Exchange2010_SP2、または Exchange2013 です。
  
## <a name="remarks"></a>注釈

この要素が存在しない場合は、最新のサービス バージョンが使用されます。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
  
[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

