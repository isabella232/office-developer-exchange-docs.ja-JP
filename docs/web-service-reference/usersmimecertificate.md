---
title: UserSMIMECertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 66e6b4ba-368d-4469-bd47-e59441b7d64d
description: UserSMIMECertificate 要素には、連絡先の SMIME 証明書をエンコードする値が含まれています。
ms.openlocfilehash: 7e2dbc6a9c8b04758ba99db036e237d8837850aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467656"
---
# <a name="usersmimecertificate"></a>UserSMIMECertificate

**UserSMIMECertificate**要素には、連絡先の SMIME 証明書をエンコードする値が含まれています。 
  
```XML
<UserSMIMECertificate/>
```

 **ArrayOfBinaryType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[Base64Binary](base64binary.md) <br/> |Base64 でエンコードされた値を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[連絡先](contact.md) <br/> |Exchange ストア内の連絡先アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

