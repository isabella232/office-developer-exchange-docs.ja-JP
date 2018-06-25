---
title: 構成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: 構成要素は、ユーザーのメールボックスを識別します。
ms.openlocfilehash: 9f359a2b0ba315c236d4bf189c3de321417bd390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839937"
---
# <a name="usermailbox"></a>構成

**構成**要素は、ユーザーのメールボックスを識別します。 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 **UserMailboxType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |**Id**属性のテキスト値は、メールボックスの識別子です。  <br/> |
|IsArchive  <br/> |**IsArchive**属性のテキスト値は、メールボックスは、アーカイブ メールボックスであるかどうかを示します。 テキストの値**は true** **IsArchive**属性には、メールボックスが、アーカイブ メールボックスであることを示します。 **False** **IsArchive** ] 属性の値は、メールボックスがプライマリ メールボックスであることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[メールボックス (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |true  <br/> |
   

