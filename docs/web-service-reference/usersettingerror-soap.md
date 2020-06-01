---
title: UserSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: abb175c5-4f38-4dcc-81e3-b511686862eb
description: UserSettingError 要素は、ユーザー設定を取得しようとした結果として返されるエラーを表します。
ms.openlocfilehash: 61603038ce93780f690d72226b1356b239d2002d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468608"
---
# <a name="usersettingerror-soap"></a>UserSettingError (SOAP)

**Usersettingerror**要素は、ユーザー設定を取得しようとした結果として返されるエラーを表します。 
  
```XML
<UserSettingError>
    <ErrorCode/>
    <ErrorMessage/>
    <SettingName/>
</UserSettingError>
```

 **UserSettingError**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |自動検出サービスによって返されるエラーコードを表します。  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |このメッセージは、自動検出サービスによって返されるエラーコードに関連付けられています。  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |ユーザー設定の名前を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |返すことができなかった設定に関する情報のコレクションを表します。  <br/> |
   
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



[Exchange 2013 の SOAP 自動検出 XML 要素](soap-autodiscover-xml-elements-for-exchange-2013.md)

