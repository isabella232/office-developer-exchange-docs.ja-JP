---
title: MSExchangeCertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c514f22f-be3e-4cad-ac56-bdff6bafcee6
description: MSExchangeCertificate 要素には、連絡先の Microsoft 証明書をエンコードExchange値が含まれている。
ms.openlocfilehash: 14993f2a1067334bba5c8980bc57eaff550f09d0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529795"
---
# <a name="msexchangecertificate"></a>MSExchangeCertificate

**MSExchangeCertificate** 要素には、連絡先の Microsoft 証明書をエンコードExchange値が含まれている。 
  
```XML
<MSExchangeCertificate/>
```

 **ArrayOfBinaryType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[Base64Binary](base64binary.md) <br/> |Base64 でエンコードされた値を含む。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[Contact](contact.md) <br/> |ストア内の連絡先アイテムExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

