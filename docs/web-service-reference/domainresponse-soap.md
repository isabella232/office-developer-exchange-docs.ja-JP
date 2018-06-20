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
description: DomainResponse 要素には、指定したドメインの指定された設定が含まれています。
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760149"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

**DomainResponse**要素には、指定したドメインの指定された設定が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |返されませんでしたの設定に関するエラー情報が含まれています。  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |自動検出要求の送信、または、自動検出応答によって返されるドメインの設定を表します。  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |リダイレクトのターゲットを識別します。 ターゲットは、URL または電子メール アドレスのいずれかを使用できます。  <br/> |
|[エラー コード (SOAP)](errorcode-soap.md) <br/> |特定の要求に関連付けられているエラー コードを指定します。  <br/> |
|[エラー メッセージ (SOAP)](errormessage-soap.md) <br/> |特定の要求に関連付けられているエラー メッセージを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |**DomainResponse**要素の配列が含まれています。 **DomainResponse**の各要素には、指定したユーザーの要求された設定が含まれています。  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |ドメインごとの応答が含まれています。  <br/> |
   
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

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)

