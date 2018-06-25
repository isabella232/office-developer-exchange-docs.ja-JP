---
title: 応答 (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: 応答要素は、個々 のドメインの GetDomainSettings 呼び出しへの応答を表します。
ms.openlocfilehash: 316d77104894cf5ed9121e7dab1c38646765c948
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833169"
---
# <a name="response-getdomainsettings-soap"></a>応答 (GetDomainSettings) (SOAP)

**応答**要素は、個々 のドメインの**GetDomainSettings**呼び出しへの応答を表します。 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 **GetDomainSettingsResponse**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |**GetDomainSettings**要求で要求された各ドメインへの応答が含まれています。  <br/> |
|[エラー コード (SOAP)](errorcode-soap.md) <br/> |該当する場合、応答に関連付けられているエラー コードが含まれています。  <br/> |
|[エラー メッセージ (SOAP)](errormessage-soap.md) <br/> |該当する場合、応答に関連付けられているエラー メッセージが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |呼び出し元に、ドメイン構成設定を返します。  <br/> |
   
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



[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

