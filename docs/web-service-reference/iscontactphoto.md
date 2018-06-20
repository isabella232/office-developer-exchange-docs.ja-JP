---
title: IsContactPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsContactPhoto
api_type:
- schema
ms.assetid: ae36b5f9-a787-4863-9dbc-258ad724801d
description: IsContactPhoto 要素は、添付ファイルに連絡先の写真があるかどうかを示します。
ms.openlocfilehash: a015cd9bdb34ea9275952d5fe252a30cacf888ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831999"
---
# <a name="iscontactphoto"></a>IsContactPhoto

**IsContactPhoto**要素は、添付ファイルに連絡先の写真があるかどうかを示します。 
  
```xml
<IsContactPhoto>true or false</IsContactPhoto>
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
|[FileAttachment](fileattachment.md) <br/> |Exchange ストア内のアイテムに関連付けられているファイルを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には、 **true**または**false**のいずれかができます。 既定値は、 **false を指定**します。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

