---
title: SetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 8aa4025b-38df-4d63-a6a5-c3b932bec26e
description: SetUserOofSettingsResponse 要素には、Setuseroofsettingsresponse 要求メッセージの試行の結果が含まれています。
ms.openlocfilehash: 9b02d905f82488965f5ae0514a52eb6062aaff7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466130"
---
# <a name="setuseroofsettingsresponse"></a>SetUserOofSettingsResponse

**Setuseroofsettingsresponse**要素には、 [Setuseroofsettingsresponse 要求](setuseroofsettingsrequest.md)メッセージの試行の結果が含まれています。 
  
```xml
<SetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
<SetUserOofSettingsResponse>
```

 **SetUserOofSettingsResponse**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> |応答状態に関する説明情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SetUserOofSettings 操作](setuseroofsettings-operation.md)

