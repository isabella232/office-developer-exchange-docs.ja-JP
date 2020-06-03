---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: UserConfigurationProperties 要素は、GetUserConfiguration 操作で取得するプロパティの種類を指定します。
ms.openlocfilehash: af6bee64516a7410d96ecc7581e8e819f550ddc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466494"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

**Userconfigurationproperties**要素は、getuserconfiguration 操作で取得するプロパティの種類を指定します。 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 **UserConfigurationPropertyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserConfiguration](getuserconfiguration.md) <br/> |ユーザー構成オブジェクトを取得する要求を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **Userconfigurationproperties**要素に指定できる値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|ID  <br/> |Identifier プロパティを指定します。  <br/> |
|Dictionary  <br/> |ディクショナリのプロパティの種類を指定します。  <br/> |
|XmlData  <br/> |XML データプロパティの種類を指定します。  <br/> |
|BinaryData  <br/> |バイナリデータのプロパティの種類を指定します。  <br/> |
|すべて  <br/> |識別子、辞書、XML データ、およびバイナリデータのプロパティの種類を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

