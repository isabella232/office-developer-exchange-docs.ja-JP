---
title: Exchange の偽装と EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e1ea63c-eb29-43d2-827f-2f2b1846483b
description: Exchange サービス アプリケーションで偽装を使用する方法とタイミングについて説明します。
ms.openlocfilehash: f8a215874475034f0d147b80a05cae414e6438f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759073"
---
# <a name="impersonation-and-ews-in-exchange"></a><span data-ttu-id="37608-103">Exchange の偽装と EWS</span><span class="sxs-lookup"><span data-stu-id="37608-103">Impersonation and EWS in Exchange</span></span>

<span data-ttu-id="37608-104">Exchange [サービス アプリケーション](ews-application-types.md)で偽装を使用する方法とタイミングについて説明します。</span><span class="sxs-lookup"><span data-stu-id="37608-104">Learn how and when to use impersonation in your Exchange [service applications](ews-application-types.md).</span></span>
  
<span data-ttu-id="37608-105">次の 3 つの方法のいずれかで、他のユーザーのメールボックスにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="37608-105">You can enable users to access other users' mailboxes in one of three ways:</span></span>
  
- <span data-ttu-id="37608-106">代理人を追加し、各代理人にアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="37608-106">By adding delegates and specifying permissions for each delegate.</span></span>
    
- <span data-ttu-id="37608-107">フォルダーのアクセス許可を直接変更します。</span><span class="sxs-lookup"><span data-stu-id="37608-107">By modifying folder permissions directly.</span></span>
    
- <span data-ttu-id="37608-108">偽装を使用します。</span><span class="sxs-lookup"><span data-stu-id="37608-108">By using impersonation.</span></span>
    
<span data-ttu-id="37608-p101">委任またはフォルダーのアクセス許可を使った方法よりも偽装を使った方法を選択するのが最善かどうかを判断するうえで、次のガイドラインが役に立ちます。</span><span class="sxs-lookup"><span data-stu-id="37608-p101">When should you choose impersonation over delegation or folder permissions? The following guidelines will help you decide:</span></span>
  
- <span data-ttu-id="37608-111">フォルダーに対してユーザー アクセスを提供するものの、ユーザーに "代理人として送信する" アクセス許可を付与しない場合は、フォルダーのアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="37608-111">Use folder permissions when you want to provide a user access to a folder but do not want the user to have "send on behalf of" permissions.</span></span> 
    
- <span data-ttu-id="37608-p102">1 人のユーザーに別のユーザーの代わりに作業を実行するためのアクセス許可を付与する場合は、代理人アクセスを使用します。通常、これは 1 対 1 または 1 対多のアクセス許可です。たとえば、単一の管理アシスタントが管理者の予定表を管理している、または単一の会議室スケジューラが会議室のグループの予定表を管理している場合などです。</span><span class="sxs-lookup"><span data-stu-id="37608-p102">Use delegate access when you want to give one user permission to perform work on behalf of another user. Typically, this is a one-to-one or one-to-a-few permission - for example, a single administrative assistant managing the calendar for an administrator, or a single room scheduler managing the calendars for a group of meeting rooms.</span></span>
    
- <span data-ttu-id="37608-114">複数のメールボックスにアクセスしてメールボックスの所有者として "操作を行う" 必要のあるサービス アプリケーションがある場合は、偽装を使用します。</span><span class="sxs-lookup"><span data-stu-id="37608-114">Use impersonation when you have a service application that needs to access multiple mailboxes and "act as" the mailbox owner.</span></span>
    
<span data-ttu-id="37608-p103">偽装は、1 つのサービス アカウントにデータベース内のすべてのメールボックスへのアクセスを簡単に許可できるため、複数のメールボックスを処理するときに最適です。委任、およびフォルダーのアクセス許可は、各メールボックスに個別にアクセス許可を追加する必要があるため、少数のユーザーにのみアクセス許可を付与する場合に最適です。図 1 は、それぞれのアクセス許可の種類ごとの違いを示しています。</span><span class="sxs-lookup"><span data-stu-id="37608-p103">Impersonation is the best choice when you're dealing with multiple mailboxes because you can easily grant one service account access to every mailbox in a database. Delegation and folder permissions are best when you're only granting access to a few users, because you have to add permissions individually to each mailbox. Figure 1 shows some of the differences between each type of access.</span></span>
  
<span data-ttu-id="37608-118">**図 1. 他のユーザーのメールボックスにアクセスする方法**</span><span class="sxs-lookup"><span data-stu-id="37608-118">**Figure 1. Ways to access other users' mailboxes**</span></span>

![メールボックスのアクセス タイプ、各タイプのメールボックス所有者と代理人の関係、およびアクセス許可のタイプを示す図。委任用のアクセス許可またはフォルダー アクセス許可のために送信します。偽装のためのアクセス許可として送信します。](media/Ex15_Delegate_Overview.png)
  
<span data-ttu-id="37608-p105">偽装は、Exchange Online、Office 365 の一部としての Exchange Online、およびオンプレミス バージョンの Exchange に接続し、メールのアーカイブ、休暇中のユーザーへの OOF の自動設定、アプリケーションがメールボックスの所有者として動作する必要のある他のすべてのタスクなどの操作を実行するアプリケーションに最適です。アプリケーションでメッセージを送信するのに偽装を使用すると、メールがメールボックスの所有者から送信されたものとして表示されます。サービス アカウントによって送信されたメールであることを受信者が確認する手段はありません。一方、委任は、別のメールボックス アカウントに対して、メールボックスの所有者の代わりに動作するためのアクセス許可を付与します。代理人によってメール メッセージが送信される場合、"from" 値はメールボックスの所有者になり、"sender" 値はメールを送信した代理人になります。</span><span class="sxs-lookup"><span data-stu-id="37608-p105">Impersonation is ideal for applications that connect to Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange and perform operations, such as archiving email, setting OOF automatically for users on vacation, or any other task that requires that the application act as the owner of a mailbox. When an application uses impersonation to send a message, the email appears to be sent from the mailbox owner. There is no way for the recipient to know the mail was sent by the service account. Delegation, on the other hand, gives another mailbox account permission to act on behalf of a mailbox owner. When an email message is sent by a delegate, the "from" value identifies the mailbox owner, and the "sender" value identifies the delegate that sent the mail.</span></span> 
  
## <a name="security-considerations-for-impersonation"></a><span data-ttu-id="37608-127">偽装のセキュリティの考慮事項</span><span class="sxs-lookup"><span data-stu-id="37608-127">Security considerations for impersonation</span></span>

<span data-ttu-id="37608-p106">偽装を使用すると、発信者は指定されたユーザー アカウントを偽装できます。これにより、発信者は自分のアカウントに関連付けられているアクセス許可ではなく、偽装されたアカウントに関連付けられているアクセス許可を使用して操作を実行できます。このため、次のセキュリティの考慮事項に留意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="37608-p106">Impersonation enables a caller to impersonate a given user account. This enables the caller to perform operations by using the permissions that are associated with the impersonated account, instead of the permissions that are associated with the caller's account. For this reason, you should be aware of the following security considerations:</span></span>
  
- <span data-ttu-id="37608-131">Exchange サーバー管理者によって **ApplicationImpersonation** 役割が付与されているアカウントのみが偽装を使用できます。</span><span class="sxs-lookup"><span data-stu-id="37608-131">Only accounts that have been granted the **ApplicationImpersonation** role by an Exchange server administrator can use impersonation.</span></span> 
    
- <span data-ttu-id="37608-p107">指定されたアカウントのグループに偽装を限定する管理スコープを作成する必要があります。管理スコープを作成しないと、 **ApplicationImpersonation** 役割が組織内のすべてのアカウントに付与されます。</span><span class="sxs-lookup"><span data-stu-id="37608-p107">You should create a management scope that limits impersonation to a specified group of accounts. If you do not create a management scope, the **ApplicationImpersonation** role is granted to all accounts in an organization.</span></span> 
    
- <span data-ttu-id="37608-p108">通常、 **ApplicationImpersonation** 役割はユーザー アカウントではなく、特定のアプリケーションまたはアプリケーションのグループ専用のサービス アカウントに付与されます。必要に応じて、必要な数のサービス アカウントを作成できます。</span><span class="sxs-lookup"><span data-stu-id="37608-p108">Typically, the **ApplicationImpersonation** role is granted to a service account dedicated to a particular application or group of applications, rather than a user account. You can create as many or as few service accounts as you need.</span></span> 
    
<span data-ttu-id="37608-136">[偽装の構成](how-to-configure-impersonation.md)についての詳細を読むこともできますが、Exchange 管理者と相談して、必要とするサービス アカウントが組織のセキュリティ要件を満たす[アクセス許可やアクセス](http://technet.microsoft.com/ja-jp/library/dd351175%28v=exchg.150%29.aspx)を持つものとして作成されるようにしなければなりません。</span><span class="sxs-lookup"><span data-stu-id="37608-136">You can read more about [configuring impersonation](how-to-configure-impersonation.md), but you should work with your Exchange administrator to ensure that the service accounts that you need are created with the [permissions and access](http://technet.microsoft.com/ja-jp/library/dd351175%28v=exchg.150%29.aspx) that meet the security requirements of your organization.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="37608-137">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="37608-137">In this section</span></span>

- [<span data-ttu-id="37608-138">偽装を構成します。</span><span class="sxs-lookup"><span data-stu-id="37608-138">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="37608-139">偽装するアカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="37608-139">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="37608-140">Exchange の偽装を使用して予定を追加します。</span><span class="sxs-lookup"><span data-stu-id="37608-140">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a><span data-ttu-id="37608-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="37608-141">See also</span></span>


- [<span data-ttu-id="37608-142">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="37608-142">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="37608-143">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="37608-143">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
    
- [<span data-ttu-id="37608-144">Exchange 2013 アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37608-144">Exchange 2013 Permissions</span></span>](http://technet.microsoft.com/ja-jp/library/dd351175%28v=exchg.150%29.aspx)
    

