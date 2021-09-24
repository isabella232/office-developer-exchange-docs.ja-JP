---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: MailboxStat 要素は、探索検索で検索されたメールボックスの統計情報を指定します。
ms.openlocfilehash: d48f033df4cfec47313ce690acd19d916b963c00
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522811"
---
# <a name="mailboxstat"></a>MailboxStat

**MailboxStat 要素** は、探索検索で検索されたメールボックスの統計情報を指定します。 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

**MailboxStatisticsItemType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[MailboxId](mailboxid.md)  | [DisplayName (string)](displayname-string.md)  | [ItemCount](itemcount.md)  | [サイズ (長)](size-long.md)
  
### <a name="parent-elements"></a>親要素

[MailboxStats](mailboxstats.md)
  
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
   

