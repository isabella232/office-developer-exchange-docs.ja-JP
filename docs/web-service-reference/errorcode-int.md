---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: ErrorCode 要素は、メールボックスに対して実行された失敗した検索のエラー コードを指定します。
ms.openlocfilehash: 25a0b14ecefce76707a8dfa73f99d8b93b445af7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530838"
---
# <a name="errorcode-int"></a>ErrorCode (int)

**ErrorCode 要素** は、メールボックスに対して実行された失敗した検索のエラー コードを指定します。 
  
```XML
<ErrorCode></ErrorCode>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FailedMailbox](failedmailbox.md) <br/> |メールボックスの保留状態を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ErrorCode 要素の **テキスト値** は、メールボックスに対して実行された失敗した検索に対して返されるエラー コードです。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

