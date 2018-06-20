---
title: ResponseCode (InvalidRecipientResponseCodeType)
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
description: ResponseCode 要素は、受信者が有効な理由についての情報を提供します。
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

**ResponseCode**要素は、受信者が有効な理由についての情報を提供します。 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **InvalidRecipientResponseCodeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |受信者が有効な理由については、無効な受信者の SMTP アドレスが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **ResponseCode**要素の値を一覧します。 
  
|**コード**|**説明**|
|:-----|:-----|
|OtherError  <br/> |エラーが、別のエラー応答コードが指定されていないことを示します。  <br/> |
|RecipientOrganizationNotFederated  <br/> |共有関係は利用できない受信者の SMTP 電子メール アドレスで指定された組織のことを示します。  <br/> |
|CannotObtainTokenFromSTS  <br/> |トークン サーバからセキュリティ トークンの取得に問題があったことを示します。  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |システム管理者が指定された受信者との共有をブロックするシステム ポリシーを設定することを示します。  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |指定された受信者によって使用されるセキュリティ トークン サービスが正常であることを示します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

