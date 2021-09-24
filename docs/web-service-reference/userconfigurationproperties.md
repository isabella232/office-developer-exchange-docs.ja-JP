---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: UserConfigurationProperties 要素は、GetUserConfiguration 操作で取得するプロパティの種類を指定します。
ms.openlocfilehash: 0aed3ffc680ac881410469fe762349739ba924a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515006"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

**UserConfigurationProperties 要素** は、GetUserConfiguration 操作で取得するプロパティの種類を指定します。 
  
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

次の表に **、UserConfigurationProperties 要素に使用できる値を示** します。 
  
|**値**|**説明**|
|:-----|:-----|
|ID  <br/> |識別子プロパティを指定します。  <br/> |
|Dictionary  <br/> |ディクショナリ プロパティの種類を指定します。  <br/> |
|XmlData  <br/> |XML データ プロパティの種類を指定します。  <br/> |
|BinaryData  <br/> |バイナリ データ プロパティの種類を指定します。  <br/> |
|すべて  <br/> |識別子、辞書、XML データ、およびバイナリ データ プロパティの種類を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

