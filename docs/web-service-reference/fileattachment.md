---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: FileAttachment 要素は、Exchange ストア内のアイテムに関連付けられているファイルを表します。
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760484"
---
# <a name="fileattachment"></a>FileAttachment

**FileAttachment**要素は、Exchange ストア内のアイテムに関連付けられているファイルを表します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |添付ファイルを識別します。  <br/> |
|[名 (AttachmentType)](name-attachmenttype.md) <br/> |添付ファイルの名前を表します。  <br/> |
|[ContentType](contenttype.md) <br/> |添付ファイルのコンテンツの多目的インターネット メール拡張 (MIME) の種類について説明します。  <br/> |
|[ContentId](contentid.md) <br/> |添付ファイルの内容の識別子を表します。 [ContentId](contentid.md)は、任意の文字列値に設定できます。 アプリケーションは、独自の識別メカニズムを実装するために、 [ContentId](contentid.md)を使用できます。  <br/> |
|[ContentLocation](contentlocation.md) <br/> |統一リソース識別子 (URI) の添付ファイルのコンテンツの場所に対応するが含まれています。  <br/> |
|[Size](size.md) <br/> |添付ファイルのバイト単位でサイズを表します。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |添付ファイルが最後に変更されたときを表します。  <br/> |
|[IsInline](isinline.md) <br/> |添付ファイルの項目内でのインラインで表示されているかどうかを表します。  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |添付ファイルが連絡先の写真であるかどうかを示します。  <br/> |
|[コンテンツ](content.md) <br/> |添付ファイルの Base64 でエンコードされた内容が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

