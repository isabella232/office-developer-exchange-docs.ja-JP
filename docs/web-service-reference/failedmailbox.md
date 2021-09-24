---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: FailedMailbox 要素は、検索で失敗したメールボックスのエラー メッセージを指定します。
ms.openlocfilehash: 5e2bfbce5da35ecacd1757a9c612ed226af963ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535259"
---
# <a name="failedmailbox"></a>FailedMailbox

**FailedMailbox 要素** は、検索で失敗したメールボックスのエラー メッセージを指定します。 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 **FailedSearchMailboxType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Mailbox (string)](mailbox-string.md) <br/> |メールボックスの識別子が含まれる。  <br/> |
|[ErrorCode (int)](errorcode-int.md) <br/> |検索に失敗したメールボックスのエラー コードを指定します。  <br/> |
|[ErrorMessage](errormessage.md) <br/> |検証エラーの理由を表します。  <br/> |
|[IsArchive](isarchive.md) <br/> |メールボックスがアーカイブであるかどうかを示すブール値を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FailedMailboxes](failedmailboxes.md) <br/> |失敗したメールボックスの配列を指定します。  <br/> |
   
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

