---
title: CChkSGFiles.ErrTerm 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: '最終更新日: 2013 年2月25日'
ms.openlocfilehash: 12b07fba69054d327c7250bbf83e4c77016e8b3f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466200"
---
# <a name="cchksgfileserrterm-function"></a>CChkSGFiles.ErrTerm 関数
  
**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
すべてのデータベース ページとログが正常に検証されたかどうかを示す、データベースとログの検証の全体的な状態を提供します。
  
> [!IMPORTANT]
> ストレージグループは、Exchange 2013 では使用できません。 Exchange Server 2010 より前のバージョンの Exchange でデータベースおよびストレージグループとの下位互換性を維持するために、CHKSGFILES API ではストレージグループを指定することができます。 Exchange 2013 データベースに対して CHKSGFILES を実行するときは、ストレージグループ識別子を指定するパラメーターを空の文字列に設定する必要があります。 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>パラメーター

### <a name="ulflags"></a>ulFlags
  
オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>戻り値

[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。 
  
## <a name="remarks"></a>注釈

**CChkSGFiles** オブジェクトは、**ErrInit** 関数に登録されているすべてのデータベースが実際にチェックされたかどうかを判別します。 このオブジェクトは **ErrCheckDbPages** 関数を使って、**ErrCheckDbHeaders** 関数で示されているのと同じ数のデータベース ページが実際に検証されたことを確認します。 各データベースで適切な数のページが正常にチェックされていない場合、**ErrTerm** 関数はエラーを返します。 
  
**ErrCheckDbPages** でチェックしたデータベース ページの数が **ErrCheckDbHeaders** で示されている数よりも少ない場合、この関数は Windows イベント ログにエラーを作成し、**ErrTerm** がエラーを返します。 
  
**ErrCheckDbPages** でチェックしたデータベース ページの数が **ErrCheckDbHeaders** で示されている数よりも多い場合、この関数は、アプリケーションが一部のデータベース ページを複数回にわたり不必要にチェックした可能性を示す警告を Windows イベント ログに作成します。 ただし、この場合には **ErrTerm** 関数は成功します。 
  
また、**CChkSGFiles** オブジェクトは **ErrInit** に登録されたログ ファイルが実際にチェックされたかどうかを判別します。 正常にチェックされなかったログがあると、**ErrTerm** 関数はエラーを返します。 
  
**ErrTerm** がエラーを返す場合、この関数は **ErrInit** に登録されているすべてのデータベースの検証状態をチェックしますが、このエラーが最初に検出されます。
  
マルチスレッドアプリケーションで CHKSGFILES を使用している場合は、アプリケーションの単一スレッドの部分で**Errterm**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに1回だけ呼び出すことができます。 
  
## <a name="requirements"></a>Requirements

Exchange 2013 には、CHKSGFILES の64ビットバージョンのみが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

