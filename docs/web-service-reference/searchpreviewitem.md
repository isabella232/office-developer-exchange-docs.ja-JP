---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: SearchPreviewItem 要素は、探索検索のアイテム プレビューを指定します。
ms.openlocfilehash: 7ecc034de3386ed35f0071403c013e91b79d13c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534303"
---
# <a name="searchpreviewitem"></a>SearchPreviewItem

**SearchPreviewItem** 要素は、探索検索のアイテム プレビューを指定します。 
  
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

 **SearchPreviewItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ID (ItemIdType)](id-itemidtype.md)  | [メールボックス (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md)  | [ParentId](parentid.md)  | [ItemClass](itemclass.md)  | [UniqueHash](uniquehash.md)  | [SortValue](sortvalue.md)  | [OwaLink](owalink.md)  | [送信者 (文字列)](sender-string.md)  | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md)  | [CcRecipients](ccrecipients.md)  | [BccRecipients](bccrecipients.md)  | [CreatedTime](createdtime.md)  | [ReceivedTime](receivedtime.md)  | [SentTime](senttime.md)  | [件名](subject.md)  | [サイズ (長)](size-long.md)  | [プレビュー](preview-ex15websvcsotherref.md)  | [重要度](importance.md)  | [読み取り](read.md)  | [HasAttachment](hasattachment.md)  | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)
  
### <a name="parent-elements"></a>親要素

[Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

