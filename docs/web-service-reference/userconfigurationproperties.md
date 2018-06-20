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
description: UserConfigurationProperties 要素は、GetUserConfiguration の操作で取得するプロパティの型を指定します。
ms.openlocfilehash: 4f993765bb7c36f28a41a3f2fa7e28698a3f709e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839928"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

**UserConfigurationProperties**要素は、GetUserConfiguration の操作で取得するプロパティの型を指定します。 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 **UserConfigurationPropertyType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserConfiguration](getuserconfiguration.md) <br/> |ユーザーの構成オブジェクトを取得する要求を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **UserConfigurationProperties**要素の値を一覧します。 
  
|**値**|**説明**|
|:-----|:-----|
|ID  <br/> |識別子のプロパティを指定します。  <br/> |
|Dictionary  <br/> |ディクショナリ プロパティの種類を指定します。  <br/> |
|XmlData  <br/> |プロパティの XML データ型を指定します。  <br/> |
|データ  <br/> |バイナリ データのプロパティの種類を指定します。  <br/> |
|All  <br/> |識別子、ディクショナリ、XML データ、およびバイナリ データのプロパティの種類を指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

