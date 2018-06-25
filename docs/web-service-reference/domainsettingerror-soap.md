---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: DomainSettingError 要素は、ドメインの設定を取得中に発生したエラーを表します。 これは、GetDomainSettings 要求のエラーを表します。
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760158"
---
# <a name="domainsettingerror-soap"></a>DomainSettingError (SOAP)

**DomainSettingError**要素は、ドメインの設定を取得中に発生したエラーを表します。 これは、 **GetDomainSettings**要求のエラーを表します。 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 **DomainSettingError**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[エラー コード (SOAP)](errorcode-soap.md) <br/> |特定の要求に関連付けられているエラー コードを識別します。  <br/> |
|[エラー メッセージ (SOAP)](errormessage-soap.md) <br/> |特定の要求に関連付けられているエラー メッセージが含まれています。  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |設定の名前を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |返されませんでしたの設定に関するエラー情報が含まれています。  <br/> |
   
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

