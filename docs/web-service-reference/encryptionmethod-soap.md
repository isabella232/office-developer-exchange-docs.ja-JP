---
title: EncryptionMethod (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bc632c85-ec74-4a00-baec-df5973e032fa
description: EncryptionMethod 要素は、POP、IMAP、および SMTP のプロトコルに使用される暗号化メソッドを表します。
ms.openlocfilehash: 5062d357a54019a576e391e1be4d4e8dfcc6e38d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760274"
---
# <a name="encryptionmethod-soap"></a>EncryptionMethod (SOAP)

**EncryptionMethod**要素は、POP、IMAP、および SMTP のプロトコルに使用される暗号化メソッドを表します。 
  
```XML
<EncryptionMethod/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ProtocolConnection (SOAP)](protocolconnection-soap.md) <br/> |サーバーの Web クライアントのプロトコル接続を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、POP、IMAP、および SMTP のプロトコルに使用する暗号化方法です。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

