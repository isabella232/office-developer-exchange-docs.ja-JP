---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: DomainResponse 要素には、指定されたドメインに対して要求された設定が含まれています。
ms.openlocfilehash: dea6e36c51ceea53201b668cfba616c03a44df86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456963"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

**Domainresponse**要素には、指定されたドメインに対して要求された設定が含まれています。 
  
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
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |返すことができなかった設定に関するエラー情報が含まれています。  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |自動検出要求で送信された、または自動検出応答によって返されたドメイン設定を表します。  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |リダイレクトのターゲットを識別します。 ターゲットには、URL または電子メールアドレスのいずれかを指定できます。  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |特定の要求に関連付けられているエラーコードを指定します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |特定の要求に関連付けられているエラーメッセージを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |**Domainresponse**要素の配列を格納します。 各**Domainresponse**要素には、指定されたユーザーに対して要求された設定が含まれています。  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |各ドメインの応答を含みます。  <br/> |
   
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

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

