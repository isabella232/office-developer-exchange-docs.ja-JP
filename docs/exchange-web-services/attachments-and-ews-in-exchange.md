---
title: Exchange の添付物と EWS
manager: sethgros
ms.date: 7/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8e4289a4-ec9d-4502-9854-c593c95d5f98
description: 添付物と、Exchange クライアントの EWS マネージ API または EWS で添付物を表す方法について説明します。
ms.openlocfilehash: e4a97873798b8252e6fc14003519ce8a0eab7ec8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758879"
---
# <a name="attachments-and-ews-in-exchange"></a>Exchange の添付物と EWS

添付物と、Exchange クライアントの EWS マネージ API または EWS で添付物を表す方法について説明します。
  
通常、添付物は、メール アイテムに関連付けられていますが、実際には、すべての EWS アイテム (子メールのメッセージ、予定表アイテム、連絡先、タスク) に添付物を含めることができます。
  
## <a name="types-of-attachments"></a>添付物の種類

EWS は、添付物をファイル添付とアイテム添付の 2 つのグループに分類します。
  
- **アイテム添付:** メール メッセージ、予定表アイテムなどの厳密に型指定された [EWS アイテム](folders-and-items-in-ews-in-exchange.md)。これらは厳密に型指定された別の EWS アイテムに添付されています。 EWS マネージ API または EWS を使用して作成できるすべての厳密に型指定されたアイテムは、アイテム添付として使用できます。 アイテム添付のコンテンツは、厳密に型指定されたアイテムであり、そのすべてのプロパティに簡単にアクセスできます。 アイテム添付はそれ自体のアイテム添付を持つことができます。そのためアイテム添付の階層 (または添付物の入れ子) を構成できます。
    
- **ファイル添付:** .txt、.jpg、.zip、.pdf などのすべてのファイル (.msg ファイルも含む)。 ファイル添付には少数のプロパティしかありませんが、その 1 つは、Base-64 でエンコードされたファイル コンテンツです。 
    
- **参照添付物:** ファイル プロバイダーによって参照される添付物 (クラウド内にあるファイルなど)。 1 つの添付物が複数のプロバイダーから参照される場合もあります。 
    
添付物をアイテムに追加またはアイテムから取得する場合、ファイル添付であるか、アイテム添付であるかによって、操作が異なります。 たとえば、アイテムにファイル添付を追加する場合は、ファイルの場所を渡すだけです。 アイテム添付として既存のアイテムを追加する場合は、既存のアイテムのプロパティまたは MIME コンテンツを新しいアイテム添付に実際にコピーする必要があります。既存のアイテムにバインドすることはできません。 そのため、添付物の 2 つの種類を区別することが重要になります。 アイテム添付とファイル添付の違いの詳細については、[このセクション](#bk_inthissection)の記事で説明します。
  
## <a name="how-are-attachments-represented-programmatically"></a>プログラムによる添付物の表示方法

添付物は、EWS のアイテムのコレクションに保存されます。 添付物コレクションは、ファイル添付またはアイテム添付、あるいはその両方で構成されています。 添付物コレクションに関するメタデータは、EWS マネージ API の [Item.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドまたは EWS の [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作を使用してアイテムを取得した場合に使用できます。ただし、添付物のコンテンツを実際に取得するには追加の呼び出しを行う必要があります。 
  
**表 1. 添付物に関するアイテムのメタデータ**

|**メタデータ エンティティ**|**EWS マネージ API のプロパティ**|**EWS の要素**|
|:-----|:-----|:-----|
|添付物のインジケーター (インライン添付のフラグを設定しない)  <br/> |[Item.HasAttachments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|添付物のコレクション  <br/> |[Item.Attachments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Attachments](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|添付ファイルの ID  <br/> |[Attachment.Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**表 2. 添付物のエンティティ**

|**添付物の種類**|**EWS マネージ API のクラス**|**EWS の要素**|
|:-----|:-----|:-----|
|ファイル添付  <br/> |[FileAttachment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](http://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|アイテム添付  <br/> |[ItemAttachment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<TItem\>](http://msdn.microsoft.com/ja-JP/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](http://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|参照添付物  <br/> |[ReferenceAttachmentType complexType (EWS)](http://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](http://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>インライン添付

インライン添付は特別な種類の添付物です。ファイル添付とアイテム添付の両方とも、インライン添付にできます。インライン添付は、本文の内容の一部として表示され、アイテムの残りの部分のコンテンツとの関係でその位置を保持します。  
  
EWS マネージ API の [IsInline](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) プロパティまたは EWS の [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) 要素が true に設定されている場合、添付物はインライン添付です。 インライン添付は、次のオプションのプロパティと要素を使用して、インライン添付の場所を識別します。 
  
- EWS マネージ API — [ContentId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx) または [ContentLocation](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx) プロパティ。 
    
- EWS — [ContentId](http://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx) または [ContentLocation](http://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx) 要素。 
    
EWS マネージ API の [HasAttachments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) プロパティと EWS の [HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) 要素には、既存のインライン添付が存在しても反映されません。これがインライン添付が隠し添付ファイルとも呼ばれる理由です。 そのため、EWS マネージ API の [IsInline](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) プロパティまたは EWS の [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) 要素を true に設定し、アイテムに他の添付物は含まれない場合、**HasAttachments** は false に設定されます。 クライアントが **HasAttachments** を使用して、メールの添付物のインジケーターまたはアイコンを設定する場合は、インライン添付を含むメールではアイコンが表示されないことに注意してください。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange で EWS を使用して添付ファイルを追加する](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して添付ファイルを取得する](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して添付ファイルを削除する](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目
<a name="bk_additionalresources"> </a>

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    
- [Exchange のメールと EWS](email-and-ews-in-exchange.md)
    

