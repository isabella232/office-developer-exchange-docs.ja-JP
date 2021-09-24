---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: IsWritable 要素は、基になる連絡先または Active Directory 受信者を書き込むかどうかを指定します。
ms.openlocfilehash: 2663e18f2589516f304930b86a717455b6ab77c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516714"
---
# <a name="iswritable"></a>IsWritable

**IsWritable 要素** は、基になる連絡先または Active Directory 受信者を書き込むかどうかを指定します。 
  
```XML
<IsWritable> true | false </IsWritable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Attribution (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>テキスト値

**IsWritable** 要素の **テキスト値が true** の場合、連絡先または Active Directory オブジェクトが書き込みアクセスに使用できます。 false の **値は** 、連絡先または Active Directory オブジェクトが書き込みアクセスに使用できない状態を示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  

