---
title: Mailbox (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: Mailbox 要素には、メールボックス識別子とユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスが含まれる。
ms.openlocfilehash: 1a2dcc08d3e1595aede21e6982b36a60e6efafb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514299"
---
# <a name="mailbox-previewitemmailboxtype"></a>Mailbox (PreviewItemMailboxType)

**Mailbox 要素** には、メールボックス識別子とユーザーのプライマリ簡易メール転送プロトコル (SMTP) アドレスが含まれる。 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

**PreviewItemMailboxType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[MailboxId](mailboxid.md)  | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)
  
### <a name="parent-elements"></a>親要素

[SearchPreviewItem](searchpreviewitem.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

