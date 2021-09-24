---
title: UserResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a48766df-4cc8-47c2-a8c1-826daec94e5a
description: UserResponses 要素には、要求された各ユーザーの構成設定が含まれる。
ms.openlocfilehash: 301706af0ad876c6e93df246c4a598636d91068d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538535"
---
# <a name="userresponses-soap"></a>UserResponses (SOAP)

**UserResponses 要素には**、要求された各ユーザーの構成設定が含まれる。 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 **ArrayOfUserResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |個々のユーザーに対する [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md) 要求への応答を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Response (SOAP)](response-soap.md) <br/> |[GetUserSettings 操作 (SOAP) 要求に対する応答を格納](getusersettings-operation-soap.md)します。  <br/> |
   
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

