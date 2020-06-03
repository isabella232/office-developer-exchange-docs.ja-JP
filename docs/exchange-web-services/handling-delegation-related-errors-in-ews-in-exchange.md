---
title: Exchange の EWS での委任に関連するエラーの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの委任に関連するエラーを処理する方法を確認します。
ms.openlocfilehash: 145783c4e7f49ed6e2aa3a2dbe0d10909e06d7e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455353"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Exchange の EWS での委任に関連するエラーの処理

Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの委任に関連するエラーを処理する方法を確認します。
  
アプリケーションで委任を使用する、または代理人を追加または削除する場合、委任に関連するエラーを処理する必要があるかもしれません。 これらのエラーは実行時、または EWS アプリケーションを開発するときに処理することができます。 これらのエラーは、EWS マネージ API の [ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 列挙型および EWS の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素によって定義されます。 
  
## <a name="delegation-related-errors"></a>委任に関連するエラー

|**エラー**|**発生するタイミング**|**処理方法**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |アクセス権のないメールボックス、フォルダー、またはアイテムで操作を実行するとき。  <br/> |[UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) EWS マネージ API メソッドまたは [UpdateDelegate](https://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) EWS 操作を呼び出し、要求を再試行することによって、代理人がフォルダーまたはアイテムにアクセスできるように代理人のアクセス許可を更新します。  <br/> |
|ErrorAccessDenied  <br/> |変更を行う十分な権限が自分にないアイテムを変更するとき。  <br/> |**UpdateDelegate** EWS マネージ API メソッドまたは **UpdateDelegate** EWS 操作を呼び出し、要求を再試行することによって、代理人のアクセス許可を更新します。  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |メールボックスの所有者をメールボックスの代理人として追加しようとするとき。  <br/> |メールボックスの所有者ではなく、[別のユーザーを代理人として追加](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)します。  <br/> |
|ErrorDelegateAlreadyExists  <br/> |代理人が既に存在する場合に代理人を追加するとき。  <br/> |メールボックスの所有者の代理人が既に存在するため、何もする必要はありません。 または、既存の代理人のアクセス許可を変更しようとする場合は、**UpdateDelegates** メソッドまたは **UpdateDelegate** 操作を使用します。  <br/> |
|ErrorNotDelegate  <br/> |メールボックスの代理アクセス許可を持たないユーザーの代理アクセス許可を変更するとき。  <br/> |ユーザーのアクセス許可を更新または削除する前に、メールボックスの[ユーザーを代理人として追加](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)します。  <br/> |
|ErrorDelegateNoUser  <br/> |Active Directory ドメイン サービス (AD DS) に含まれないユーザーの代理アクセス許可を変更するとき。  <br/> |AD DS にユーザーを作成するか、要求内の代理人の情報を修正します。  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |代理人を使用して、メールボックスの所有者の代理として通知をサブスクライブするとき。  <br/> |メールボックスの所有者として通知をサブスクライブします。  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |プリンシパルのメールボックス サーバーとは異なるサーバーのバージョンを持つ代理人からの要求を作成するとき。  <br/> |代理人を使用するか、メールボックスがメールボックスの所有者と同じサーバーのバージョンの代理人を追加します。  <br/> |
|ErrorMissingEmailAddress  <br/> |メールボックスを持たない代理人アカウントを使用して要求を作成するとき。  <br/> |メールボックスを代理人のアカウントに追加します。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)
    
- [Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

