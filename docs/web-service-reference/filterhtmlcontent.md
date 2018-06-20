---
title: FilterHtmlContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: FilterHtmlContent 要素は、アイテムまたは添付ファイルから安全でない HTML コンテンツがフィルター処理されたかどうかを指定します。
ms.openlocfilehash: db181eff9586061d728a5e4ef55a78f4955b5713
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760485"
---
# <a name="filterhtmlcontent"></a>FilterHtmlContent

**FilterHtmlContent**要素は、アイテムまたは添付ファイルから安全でない HTML コンテンツがフィルター処理されたかどうかを指定します。 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | [GetAttachment](getattachment.md)要求への応答で返される追加のプロパティを識別します。  <br/><br/>  この要素への XPath 式は、次のようにします。 <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[ItemShape](itemshape.md) <br/> | GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。  <br/> <br/> この要素への XPath 式は、次のように。 <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には、 **true**または**false**のいずれかができます。 既定値は、 **false を指定**します。 これは、ブール型のデータ型です。
  
## <a name="remarks"></a>備考

この要素はオプションです。
  
この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

