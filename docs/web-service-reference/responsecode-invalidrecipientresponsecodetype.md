---
title: 応答 Secmode (Invalid受信者応答 Secodetype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: 応答 Secな要素は、受信者が無効である理由についての情報を提供します。
ms.openlocfilehash: d78de64de7725007ec51a55dad13d1cc892a25e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529722"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>応答 Secmode (Invalid受信者応答 Secodetype)

応答**secな**要素は、受信者が無効である理由についての情報を提供します。 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **Invalid受信者応答 Secodetype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |無効な受信者の SMTP アドレスと、受信者が無効である理由についての情報を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表**に、指定**できる値を示します。 
  
|**コード**|**説明**|
|:-----|:-----|
|OtherError  <br/> |エラーが別のエラー応答コードによって指定されていないことを示します。  <br/> |
|受信者組織のフェデレーション  <br/> |受信者の SMTP 電子メールアドレスで指定されている組織との共有関係が使用できないことを示します。  <br/> |
|CannotObtainTokenFromSTS  <br/> |トークンサーバーからセキュリティトークンを取得するときに問題が発生したことを示します。  <br/> |
|Systempolicyblockssharingwithrecipient  <br/> |システム管理者が、指定された受信者との共有をブロックするシステムポリシーを設定したことを示します。  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |指定した受信者が使用する secure token service が不明であることを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

