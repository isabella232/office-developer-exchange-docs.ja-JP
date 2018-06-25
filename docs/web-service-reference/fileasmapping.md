---
title: FileAsMapping
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAsMapping
api_type:
- schema
ms.assetid: 2c98e7c6-09b0-47b3-bbf7-8c4ef9510280
description: FileAsMapping 要素は、連絡先の表示内容を構築する方法を定義します。
ms.openlocfilehash: 1ba0ae0daa56a72c29d8c0ccad64e3edae5f0b84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760486"
---
# <a name="fileasmapping"></a>FileAsMapping

**FileAsMapping**要素は、連絡先の表示内容を構築する方法を定義します。 
  
```xml
<FileAsMapping/>
```

 **FileAsMappingType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、次の文字列値の 1 つに制限されています。
  
- なし
    
- LastCommaFirst
    
- FirstSpaceLast
    
- 会社
    
- LastCommaFirstCompany
    
- CompanyLastFirst
    
- 姓名
    
- LastFirstCompany
    
- CompanyLastCommaFirst
    
- LastFirstSuffix
    
- LastSpaceFirstCompany
    
- CompanyLastSpaceFirst
    
- LastSpaceFirst
    
- DisplayName
    
- FirstName
    
- LastFirstMiddleSuffix
    
- LastName
    
- Empty
    
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[連絡先 (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[連絡先を更新](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[連絡先を削除します。](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

