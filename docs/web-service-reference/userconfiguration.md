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
description: UserConfiguration 要素は、単一のユーザーの構成オブジェクトを定義します。
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839925"
---
# <a name="userconfiguration"></a>UserConfiguration

**UserConfiguration**要素は、単一のユーザーの構成オブジェクトを定義します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザーの構成オブジェクトの名前を表します。 ユーザーの構成オブジェクトを作成するとき、この要素を使用する必要があります。  <br/> |
|[ItemId](itemid.md) <br/> |ユーザー構成オブジェクトの項目の識別子を定義します。  <br/> |
|[辞書](dictionary.md) <br/> |ユーザーの構成オブジェクトのディクショナリ プロパティのエントリのセットを定義します。  <br/> |
|[XmlData](xmldata.md) <br/> |ユーザーの構成オブジェクトの XML データのプロパティの内容が含まれています。  <br/> |
|[データ](binarydata.md) <br/> |ユーザーの構成オブジェクトのバイナリ データ プロパティのコンテンツが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |ユーザーの構成オブジェクトを作成する要求を表します。  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |ユーザーの構成オブジェクトを返す応答を表します。  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |ユーザーの構成オブジェクトを更新する要求を表します。  <br/> |
   
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

