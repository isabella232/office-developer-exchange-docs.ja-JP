---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: FailedMailbox 要素は、検索に失敗したメールボックスは、エラー メッセージを指定します。
ms.openlocfilehash: a4f5cd975eba121dd1d8d918b638d34f907588a8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760464"
---
# <a name="failedmailbox"></a>FailedMailbox

**FailedMailbox**要素は、検索に失敗したメールボックスは、エラー メッセージを指定します。 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 **FailedSearchMailboxType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[メールボックス (文字列)](mailbox-string.md) <br/> |メールボックスの識別子が含まれています。  <br/> |
|[エラー コード (int)](errorcode-int.md) <br/> |検索に失敗したメールボックスのエラー コードを指定します。  <br/> |
|[エラー メッセージ](errormessage.md) <br/> |検証エラーの原因を表します。  <br/> |
|[IsArchive](isarchive.md) <br/> |メールボックスがアーカイブであるかどうかを示すブール値を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FailedMailboxes](failedmailboxes.md) <br/> |失敗したメールボックスの配列を指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

