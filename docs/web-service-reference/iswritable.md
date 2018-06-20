---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: IsWritable 要素は、基になっている取引先担当者または Active Directory の受信者に書き込むことがあるかどうかを指定します。
ms.openlocfilehash: 03f258d01ecfc12dfa4e09ac88f4a75340d2acf3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832158"
---
# <a name="iswritable"></a>IsWritable

**IsWritable**要素は、基になっている取引先担当者または Active Directory の受信者に書き込むことがあるかどうかを指定します。 
  
```XML
<IsWritable> true | false </IsWritable>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[属性 (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>テキスト値

**True** **IsWritable**要素のテキスト値は、取引先担当者または Active Directory オブジェクトは、書き込みアクセスに使用できることを示します。 値が**false**のないことを示します、取引先担当者または Active Directory オブジェクトの書き込みアクセスに使用できます。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

