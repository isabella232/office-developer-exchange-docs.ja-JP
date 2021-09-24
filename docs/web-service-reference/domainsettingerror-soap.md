---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: DomainSettingError 要素は、ドメイン設定の取得中に発生したエラーを表します。 これは、GetDomainSettings 要求からのエラーを表します。
ms.openlocfilehash: d2d7e1fc1509ade88de0013cb9e4ff54712d0f56
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530148"
---
# <a name="domainsettingerror-soap"></a>DomainSettingError (SOAP)

**DomainSettingError** 要素は、ドメイン設定の取得中に発生したエラーを表します。 これは **、GetDomainSettings 要求からのエラーを表** します。 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 **DomainSettingError**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |特定の要求に関連付けられているエラー コードを識別します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |特定の要求に関連付けられているエラー メッセージが含まれる。  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |設定の名前を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |返されない設定のエラー情報が含まれる。  <br/> |
   
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

