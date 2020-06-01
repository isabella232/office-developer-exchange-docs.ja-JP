---
title: Searchプレビューアイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: Searchpreview Item 要素は、探索検索のアイテムプレビューを指定します。
ms.openlocfilehash: ab48353b0ffaf4bc3b9409f1a620d145bffc7a13
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466935"
---
# <a name="searchpreviewitem"></a>Searchプレビューアイテム

**Searchpreview item**要素は、探索検索のアイテムプレビューを指定します。 
  
```XML
<SearchPreviewItem>
   <Id/>
   <Mailbox/>
   <ParentId/>
   <ItemClass/>
   <UniqueHash/>
   <SortValue/>
   <OwaLink/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <CreatedTime/>
   <ReceivedTime/>
   <SentTime/>
   <Subject/>
   <Size/>
   <Preview/>
   <Importance/>
   <Read/>
   <HasAttachment/>
   <ExtendedProperties/>
</SearchPreviewItem>
```

 **Searchプレビュー Itemtype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ID (ItemIdType)](id-itemidtype.md)  | [メールボックス (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md)  | [ParentId](parentid.md)  | [Itemclass](itemclass.md)  | [UniqueHash](uniquehash.md)  | [Sortvalue](sortvalue.md)  | [Owalink](owalink.md)  | [Sender (文字列)](sender-string.md)  | [Torの pipi(ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md)  | [Ccrecipients](ccrecipients.md)  |  イベント[Bccrecipients](bccrecipients.md)  |  イベント[ランタイム](createdtime.md)  | [ReceivedTime](receivedtime.md)  | [時間](senttime.md)  | [件名](subject.md)  | [サイズ (長い)](size-long.md)  | [プレビュー](preview-ex15websvcsotherref.md)  | [重要度](importance.md)  | [読み取り](read.md)  | [Hasattachment](hasattachment.md)  | [Extendedproperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)
  
### <a name="parent-elements"></a>親要素

[アイテム (Arrayofsearchプレビュー Itemstype)](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

