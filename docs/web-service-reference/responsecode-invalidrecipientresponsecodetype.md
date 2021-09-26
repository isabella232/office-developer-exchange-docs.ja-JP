---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: ResponseCode 要素は、受信者が無効である理由に関する情報を提供します。
ms.openlocfilehash: 33cd05aca672e250f288aec72d876734132d2e36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544809"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

**ResponseCode 要素は**、受信者が無効である理由に関する情報を提供します。 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **InvalidRecipientResponseCodeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |無効な受信者の SMTP アドレスと、受信者が無効である理由に関する情報が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、ResponseCode 要素に使用できる **値を示** します。 
  
|**コード**|**説明**|
|:-----|:-----|
|OtherError  <br/> |エラーが別のエラー応答コードで指定されていないかどうかを示します。  <br/> |
|RecipientOrganizationNotFederated  <br/> |受信者の SMTP 電子メール アドレスで指定された組織と共有関係が利用できないかどうかを示します。  <br/> |
|CannotObtainTokenFromSTS  <br/> |トークン サーバーからセキュリティ トークンを取得する際に問題が発生したかどうかを示します。  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |システム管理者が、指定した受信者との共有をブロックするシステム ポリシーを設定しました。  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |指定した受信者が使用するセキュリティで保護されたトークン サービスが不明な状態を示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

