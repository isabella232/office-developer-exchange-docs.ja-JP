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
description: IsContactPhoto 要素は、添付ファイルが連絡先の画像であるかどうかを示します。
ms.openlocfilehash: f60e558ab4f20b59c1d5ae51f9dfca430feeff00
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455549"
---
# <a name="iscontactphoto"></a>IsContactPhoto

**Iscontactphoto**要素は、添付ファイルが連絡先の画像であるかどうかを示します。 
  
```xml
<IsContactPhoto>true or false</IsContactPhoto>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FileAttachment](fileattachment.md) <br/> |Exchange ストア内のアイテムに添付されているファイルを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素は、 **true**または**false**のいずれかになります。 既定値は **false** です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

