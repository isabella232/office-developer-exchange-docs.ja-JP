---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: UserConfiguration 要素は、1つのユーザー構成オブジェクトを定義します。
ms.openlocfilehash: 1217f5d591570c2d8df49a116b6bf35c243d1e0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468909"
---
# <a name="userconfiguration"></a>UserConfiguration

**Userconfiguration**要素は、1つのユーザー構成オブジェクトを定義します。 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 **UserConfigurationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザー構成オブジェクトの名前を表します。 この要素は、ユーザー構成オブジェクトを作成するときに使用する必要があります。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザー構成オブジェクトのアイテム識別子を定義します。  <br/> |
|[辞書](dictionary.md) <br/> |ユーザー構成オブジェクトの辞書のプロパティエントリのセットを定義します。  <br/> |
|[XmlData](xmldata.md) <br/> |ユーザー構成オブジェクトの XML データプロパティコンテンツが保存されています。  <br/> |
|[BinaryData](binarydata.md) <br/> |ユーザー構成オブジェクトのバイナリデータのプロパティコンテンツが保存されています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |ユーザー構成オブジェクトを作成するための要求を表します。  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |ユーザー構成オブジェクトを返す応答を表します。  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |ユーザー構成オブジェクトを更新する要求を表します。  <br/> |
   
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

