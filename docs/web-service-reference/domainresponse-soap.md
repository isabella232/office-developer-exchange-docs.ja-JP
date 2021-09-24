---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: DomainResponse 要素には、指定したドメインの要求された設定が含まれる。
ms.openlocfilehash: fb7288b55452d8499596ce09c3ada9cec4b88d5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517204"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

**DomainResponse 要素には**、指定したドメインの要求された設定が含まれる。 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 **DomainResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |返されない設定のエラー情報が含まれる。  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |自動検出要求で送信された、または自動検出応答によって返されたドメイン設定を表します。  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |リダイレクトのターゲットを識別します。 ターゲットには、URL または電子メール アドレスを指定できます。  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |特定の要求に関連付けられているエラー コードを指定します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |特定の要求に関連付けられているエラー メッセージを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |**DomainResponse 要素の配列を含** む。 各 **DomainResponse** 要素には、指定したユーザーに対して要求された設定が含まれる。  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |各ドメインの応答を格納します。  <br/> |
   
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

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

