---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: FileAttachment 要素は、ファイル ストア内のアイテムに添付されているファイルExchangeします。
ms.openlocfilehash: 66424fefafd2084bf0b6f45881089448593e621d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518499"
---
# <a name="fileattachment"></a>FileAttachment

**FileAttachment 要素** は、ファイル ストア内のアイテムに添付されているファイルExchangeします。 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 **FileAttachmentType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |添付ファイルを識別します。  <br/> |
|[Name (AttachmentType)](name-attachmenttype.md) <br/> |添付ファイルの名前を表します。  <br/> |
|[ContentType](contenttype.md) <br/> |添付ファイルコンテンツの多目的インターネット メール拡張機能 (MIME) の種類について説明します。  <br/> |
|[ContentId](contentid.md) <br/> |添付ファイルの内容の識別子を表します。 [ContentId は](contentid.md) 、任意の文字列値に設定できます。 アプリケーションは [ContentId を使用して](contentid.md) 、独自の識別メカニズムを実装できます。  <br/> |
|[ContentLocation](contentlocation.md) <br/> |添付ファイルのコンテンツの場所に対応する統一リソース識別子 (URI) が含まれています。  <br/> |
|[サイズ](size.md) <br/> |添付ファイルのサイズをバイト単位で表します。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |添付ファイルが最後に変更された日時を表します。  <br/> |
|[IsInline](isinline.md) <br/> |アイテム内で添付ファイルがインラインで表示されるかどうかを表します。  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |添付ファイルが連絡先画像かどうかを示します。  <br/> |
|[コンテンツ](content.md) <br/> |添付ファイルの Base64 エンコードコンテンツを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテム ストア内のアイテムに添付されているアイテムまたはファイルExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

