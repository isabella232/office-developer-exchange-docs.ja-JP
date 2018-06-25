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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758879"
---
# <a name="attachments-and-ews-in-exchange"></a>Exchange の添付物と EWS

添付物と、Exchange クライアントの EWS マネージ API または EWS で添付物を表す方法について説明します。
  
通常、添付物は、メール アイテムに関連付けられていますが、実際には、すべての EWS アイテム (子メールのメッセージ、予定表アイテム、連絡先、タスク) に添付物を含めることができます。
  
## <a name="types-of-attachments"></a>添付物の種類

EWS は、添付物をファイル添付とアイテム添付の 2 つのグループに分類します。
  
- **アイテムの添付ファイル:** 厳密に型指定された[EWS の項目](folders-and-items-in-ews-in-exchange.md)、電子メール メッセージや予定表アイテムは、別の厳密に型指定された EWS アイテムに関連付けられているなどです。 EWS のマネージ API または EWS を使用して作成できる厳密に型指定されたアイテムは、アイテムの添付ファイルとして使用できます。 アイテムの添付ファイルの内容は、すべてのプロパティに簡単にアクセスを提供する厳密に型指定されたアイテムです。 項目の添付ファイルは、項目の添付ファイルなどの添付ファイルの入れ子の階層は、独自のアイテムの添付ファイルを持つことができます。
    
- **添付ファイル:**.Txt、.jpg、.zip、.pdf などの任意のファイル、またはさらに .msg ファイル。 添付ファイルは、いくつかのプロパティでは、base 64 エンコードされたコンテンツ ファイルのうちの 1 つだけにできます。 
    
- **の添付ファイルを参照:** クラウド内のファイルなど、ファイルのプロバイダーによって参照されている添付ファイルです。 添付ファイルは、複数のプロバイダーです。 
    
追加アイテムから添付ファイルを取得すると、行うことが異なるか、添付ファイルまたはアイテムの添付ファイルであるかによって。 などのアイテムに添付ファイルを追加するを渡すことができますだけでファイルの場所にします。 アイテムの添付ファイルとして既存の項目を追加するのには実際にコピーする必要のプロパティ] または [既存項目の MIME コンテンツに、新しいアイテムの添付ファイルです。だけを既存のアイテムにバインドできません。 その 2 つの種類の添付ファイルを区別することが重要です。 項目の添付ファイルと添付ファイルの違いの詳細については、[このセクションの](#bk_inthissection)記事で説明します。
  
## <a name="how-are-attachments-represented-programmatically"></a>プログラムによる添付物の表示方法

添付ファイルは、EWS の項目をコレクションに格納されます。 添付ファイルまたはアイテムの添付ファイルの添付ファイル コレクションは構成されています。 添付ファイル コレクションに関するメタデータは、EWS のマネージ API の[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)メソッドまたは EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)操作を使用してアイテムを取得するが、追加の呼び出しが実際には、添付ファイルの内容を取得するために必要なときに使用できます。 
  
**表 1 です。添付ファイルについての項目メタデータ**

|**メタデータ エンティティ**|**EWS のマネージ API のプロパティ**|**EWS の要素**|
|:-----|:-----|:-----|
|添付物のインジケーター (インライン添付のフラグを設定しない)  <br/> |[Item.HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[添付ファイル付き](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|添付物のコレクション  <br/> |[Item.Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[添付ファイル](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|添付ファイルの ID  <br/> |[Attachment.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**表 2 になります。添付ファイルのエンティティ**

|**添付ファイルの種類**|**EWS マネージ API クラス**|**EWS の要素**|
|:-----|:-----|:-----|
|添付ファイル  <br/> |[FileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](http://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|アイテム添付  <br/> |[ItemAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<TItem\>](http://msdn.microsoft.com/en-us/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](http://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|参照添付ファイル  <br/> |[ReferenceAttachmentType complexType (EWS)](http://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](http://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>インライン添付

インライン添付は特別な種類の添付物です。ファイル添付とアイテム添付の両方とも、インライン添付にできます。インライン添付は、本文の内容の一部として表示され、アイテムの残りの部分のコンテンツとの関係でその位置を保持します。  
  
EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx)要素または指定されたマネージ API の EWS [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx)プロパティが設定されている場合、添付ファイルはインラインの添付ファイルを true にします。 インラインの添付ファイルは、インラインの添付ファイルの場所を識別するのには、次の省略可能なプロパティと要素を使用します。 
  
- EWS マネージ API では、 [ContentId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx)または[ContentLocation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx)のプロパティです。 
    
- EWS- [ContentId](http://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx)または[ContentLocation](http://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx)要素です。 
    
注は、EWS のマネージ API の[添付ファイル付き](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx)のプロパティは、EWS の[添付ファイル付き](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx)の要素を反映しない存在のインラインの添付ファイルとはインラインの添付ファイルとも呼ばれます理由非表示の添付ファイルです。 マネージ API の EWS [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx)プロパティまたは EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx)要素が true に設定すると、項目の他の添付ファイルがない、**添付ファイル付き**が false に設定されます。 クライアントは、インジケーターの添付ファイルまたは電子メールのアイコンを設定するのには**添付ファイル付き**を使用する場合は、インラインの添付ファイル付き電子メールのアイコンが表示されないことに注意します。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange EWS を使用して添付ファイルを追加します。](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して添付ファイルを取得します。](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して添付ファイルを削除します。](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目
<a name="bk_additionalresources"> </a>

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    
- [Exchange の電子メールと EWS](email-and-ews-in-exchange.md)
    

