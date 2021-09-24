---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: UserConfiguration 要素は、1 つのユーザー構成オブジェクトを定義します。
ms.openlocfilehash: 3821cabf777143de4a68d20a90cb78acedcff552
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538556"
---
# <a name="userconfiguration"></a>UserConfiguration

**UserConfiguration 要素は**、1 つのユーザー構成オブジェクトを定義します。 
  
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
|[辞書](dictionary.md) <br/> |ユーザー構成オブジェクトの辞書プロパティ エントリのセットを定義します。  <br/> |
|[XmlData](xmldata.md) <br/> |ユーザー構成オブジェクトの XML データ プロパティのコンテンツを格納します。  <br/> |
|[BinaryData](binarydata.md) <br/> |ユーザー構成オブジェクトのバイナリ データ プロパティのコンテンツを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |ユーザー構成オブジェクトを作成する要求を表します。  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |ユーザー構成オブジェクトを返す応答を表します。  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |ユーザー構成オブジェクトを更新する要求を表します。  <br/> |
   
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

