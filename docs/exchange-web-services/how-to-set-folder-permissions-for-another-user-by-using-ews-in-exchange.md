---
title: Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Exchange で EWS マネージ API または EWS を使用して、フォルダーのアクセス許可レベルを設定する方法について説明します。
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759062"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a><span data-ttu-id="a6e03-103">Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="a6e03-103">How to: Set folder permissions for another user by using EWS in Exchange</span></span>

<span data-ttu-id="a6e03-104">Exchange で EWS マネージ API または EWS を使用して、フォルダーのアクセス許可レベルを設定する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-104">Learn how to set permission levels on a folder by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="a6e03-p101">フォルダー レベルのアクセス許可によって、ユーザーは、他のユーザーのメールボックスの 1 つ以上のフォルダーにアクセス可能になります。フォルダーのアクセス許可は代理人アクセスに似ていますが、次のような相違点があります。 </span><span class="sxs-lookup"><span data-stu-id="a6e03-p101">Folder-level permissions enable users to access one or more folders in another user's mailbox. Folder permissions are similar to delegate access, but they differ in the following ways:</span></span> 
  
- <span data-ttu-id="a6e03-107">フォルダーのアクセス許可では、ユーザーに "代理人として送信" させたり、別のユーザーとして "差出人を指定して送信" したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a6e03-107">Folder permissions do not enable a user to "send on behalf of" or "send as" another user. They only enable access to folders. Users can create items in those folders, but they can’t send them.</span></span> <span data-ttu-id="a6e03-108">ユーザーは、フォルダーにのみアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-108">They only enable access to folders.</span></span> <span data-ttu-id="a6e03-109">ユーザーは、フォルダーのアイテムを作成できますが、それらを送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="a6e03-109">Users can create items in those folders, but they can't send them.</span></span>
    
- <span data-ttu-id="a6e03-110">メールボックスの任意のフォルダーで、フォルダーのアクセス許可を設定できますが、代理人を追加できるのは、予定表、連絡先、受信トレイ、履歴、メモ、タスクのフォルダーのみです。</span><span class="sxs-lookup"><span data-stu-id="a6e03-110">You can set folder permissions on any folder in the mailbox, but you can only add a delegate to the Calendar, Contacts, Inbox, Journal, Notes, and Tasks folders.</span></span>
    
- <span data-ttu-id="a6e03-111">[特定のフォルダーのアクセス許可](#bk_folderperms)の数を設定できます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-111">You can set a number of [permissions on a specific folder](#bk_folderperms). When you add a delegate, you can assign one of only five permission levels.</span></span> <span data-ttu-id="a6e03-112">代理人を追加する場合、[5 つのアクセス許可レベル](delegate-access-and-ews-in-exchange.md#bk_delegateperms)の内 1 つのみを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-112">You can set a number of permissions on a specific folder. When you add a delegate, you can assign one of only [five permission levels](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span>
    
- <span data-ttu-id="a6e03-p104">匿名ユーザーおよび既定ユーザーのフォルダーのアクセス許可を設定できます。メールが有効なアカウントにだけ代理人アクセスを付与できます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p104">You can set folder permissions for anonymous and default users. You can only grant delegate access to a mail-enabled account.</span></span>
    
<span data-ttu-id="a6e03-p105">アクセス制御エントリ (ACE) と随意アクセス制御リスト (DACL) に精通していれば、ユーザーが各フォルダーのアクセス許可のセットを 1 つだけ持てることをご存じでしょう。ユーザーにアクセス許可のセットを追加しようとすると、そのユーザーがアクセス許可のセットを既に持っている場合、エラーが返されます。フォルダーのアクセス許可を追加、削除、更新する場合、現在の DACL を取得し、任意の ACE を追加するか削除し、更新した DACL を送信します。同じユーザーに対して複数の ACE を追加することはできません。EWS マネージ API を使用してアクセス許可を更新する場合、ユーザーの現在の ACE を削除し、新しい ACE をコレクションに追加する必要があります。EWS を使用している場合は、以前の ACE のセットを新しいセットに置き換えるだけです。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p105">If you're familiar with Access Control Entries (ACEs) and Discretionary Access Control Lists (DACLs), you know that a user can only have one set of permissions for each folder. If you try to add a set of permissions for a user and they already have a set of permissions, you'll get an error. When you add, remove, or update permissions on a folder, you get the current DACL, add or remove any ACEs, and then send the updated DACL. You cannot add multiple ACEs for the same user. When you update permissions by using the EWS Managed API, you need to remove the user's current ACE and then add their new ACE to the collection. If you're using EWS, you just replace the previous set of ACEs with the new ones.</span></span>
  
<span data-ttu-id="a6e03-p106">1 つのフォルダーで複数のアクセス許可を変更する場合は、追加、削除、更新をバッチ処理することができます。複数のフォルダーでユーザーの更新をするときには、バッチ処理はできないことに注意してください。1 つのフォルダーのアクセス許可を取得するために、1 回の呼び出しが必要です。そのフォルダーに対するアクセス許可を更新するには、2 番目の呼び出しが必要です。ユーザーのアクセス許可を追加、削除、更新する場合、各タスクで、同じ 2 つのメソッド呼び出しまたは操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p106">If you're making multiple permission changes to a single folder, you can batch additions, removals, or updates —just note that you cannot batch user updates on multiple folders. One call is required to get the permissions on a single folder, and a second call is required to update the permissions on that folder. When you add, remove, or update user permissions, you use the same two method calls or operations for each task.</span></span>
  
<span data-ttu-id="a6e03-124">**表 1. フォルダー アクセス許可を設定する EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="a6e03-124">**Table 1.  EWS Managed API methods and EWS operations for setting folder permissions**</span></span>

|<span data-ttu-id="a6e03-125">目的</span><span class="sxs-lookup"><span data-stu-id="a6e03-125">If you want to…</span></span>|<span data-ttu-id="a6e03-126">使用する EWS マネージ API メソッド…</span><span class="sxs-lookup"><span data-stu-id="a6e03-126">Use this EWS Managed API method…</span></span>|<span data-ttu-id="a6e03-127">使用する EWS 操作…</span><span class="sxs-lookup"><span data-stu-id="a6e03-127">Use this EWS operation…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a6e03-128">フォルダーのアクセス許可の有効化、削除、更新</span><span class="sxs-lookup"><span data-stu-id="a6e03-128">Enable, remove, or update folder permissions</span></span>  <br/> |<span data-ttu-id="a6e03-129">[Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) の後に [Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="a6e03-129">[Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="a6e03-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) の後に [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="a6e03-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="a6e03-131">フォルダーの作成、フォルダーのアクセス許可の定義</span><span class="sxs-lookup"><span data-stu-id="a6e03-131">Create a folder and define folder permissions</span></span>  <br/> |[<span data-ttu-id="a6e03-132">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="a6e03-132">Folder.Save</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a6e03-133">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="a6e03-133">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a><span data-ttu-id="a6e03-134">フォルダーのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6e03-134">Folder permissions</span></span>
<span data-ttu-id="a6e03-135"><a name="bk_folderperms"> </a></span><span class="sxs-lookup"><span data-stu-id="a6e03-135"></span></span>

<span data-ttu-id="a6e03-p107">特定のフォルダーにフォルダーのアクセス許可を設定する場合、多くのオプションがあります。ユーザーごとにフォルダーのアクセス許可レベルを設定できます。そのレベルで DACL に対する事前定義された個別のアクセス許可のセットを追加するか、フォルダーの個別アクセス許可を設定できます。しかし、それらを混在させたり、合わせたりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p107">You have quite a few options when it comes to setting folder permissions on a specific folder. You can set a permission level on a folder for each user, which adds a set of predefined individual permissions to the DACL, or you can set individual permissions on a folder — but you can't mix and match.</span></span>
  
<span data-ttu-id="a6e03-138">次の個別アクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-138">The following individual permissions are available:</span></span>
  
- <span data-ttu-id="a6e03-139">作成可能</span><span class="sxs-lookup"><span data-stu-id="a6e03-139">Can create</span></span>
- <span data-ttu-id="a6e03-140">サブフォルダー作成可能</span><span class="sxs-lookup"><span data-stu-id="a6e03-140">Can create subfolders</span></span>    
- <span data-ttu-id="a6e03-141">フォルダーの所有者になる</span><span class="sxs-lookup"><span data-stu-id="a6e03-141">Is folder owner</span></span>    
- <span data-ttu-id="a6e03-142">フォルダーを表示可能</span><span class="sxs-lookup"><span data-stu-id="a6e03-142">Is folder visible</span></span>    
- <span data-ttu-id="a6e03-143">連絡先フォルダーにする</span><span class="sxs-lookup"><span data-stu-id="a6e03-143">Is folder contact</span></span>    
- <span data-ttu-id="a6e03-144">アイテムの編集</span><span class="sxs-lookup"><span data-stu-id="a6e03-144">Edit items</span></span>    
- <span data-ttu-id="a6e03-145">アイテムの削除</span><span class="sxs-lookup"><span data-stu-id="a6e03-145">Delete items</span></span>    
- <span data-ttu-id="a6e03-146">アイテムの参照</span><span class="sxs-lookup"><span data-stu-id="a6e03-146">Read items</span></span>
    
<span data-ttu-id="a6e03-147">さらに、次のアクセス許可レベルを使用できます。それは、表 2 に示すように個別アクセス許可と値のサブセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-147">In addition, the following permission levels are available, which define a subset of individual permissions and values, as shown in Table 3:</span></span>
  
- <span data-ttu-id="a6e03-148">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-148">None</span></span>    
- <span data-ttu-id="a6e03-149">Owner (所有者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-149">Owner</span></span>    
- <span data-ttu-id="a6e03-150">PublishingEditor (出版編集者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-150">PublishingEditor</span></span>    
- <span data-ttu-id="a6e03-151">Editor (編集者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-151">Editor</span></span>    
- <span data-ttu-id="a6e03-152">PublishingAuthor (出版著者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-152">PublishingAuthor</span></span>    
- <span data-ttu-id="a6e03-153">Author (著者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-153">Author</span></span>    
- <span data-ttu-id="a6e03-154">NoneditingAuthor (非編集著者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-154">NoneditingAuthor</span></span>    
- <span data-ttu-id="a6e03-155">Reviewer (校閲者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-155">Reviewer</span></span>    
- <span data-ttu-id="a6e03-156">共同作成者</span><span class="sxs-lookup"><span data-stu-id="a6e03-156">Contributor</span></span>   
- <span data-ttu-id="a6e03-157">Custom: この値は、アプリケーションでは設定できません。</span><span class="sxs-lookup"><span data-stu-id="a6e03-157">Custom - This value cannot be set by the application.</span></span> <span data-ttu-id="a6e03-158">個別アクセス許可のカスタム コレクションがアプリケーションに含まれている場合、サーバーはこの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-158">Custom – This value cannot be set by the application. The server sets this value if the application includes a custom collection of individual permissions.</span></span>    
- <span data-ttu-id="a6e03-159">FreeBusyTimeOnly: これは予定表フォルダーにのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-159">FreeBusyTimeOnly – This can only be set on Calendar folders.</span></span>   
- <span data-ttu-id="a6e03-160">FreeBusyTimeAndSubjectAndLocation: これは予定表フォルダーにのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-160">FreeBusyTimeAndSubjectAndLocation – This can only be set on Calendar folders.</span></span>
    
<span data-ttu-id="a6e03-161">次の表は、アクセス許可レベルに基づき、既定で適用される個別アクセス許可を示しています。</span><span class="sxs-lookup"><span data-stu-id="a6e03-161">The following table shows which individual permissions are applied by default based on permission level.</span></span>
  
<span data-ttu-id="a6e03-162">**表 2.アクセス許可レベルによる個別アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="a6e03-162">**Table 3.  Individual permissions by permission level**</span></span>

|<span data-ttu-id="a6e03-163">権限レベル</span><span class="sxs-lookup"><span data-stu-id="a6e03-163">Permission level</span></span>|<span data-ttu-id="a6e03-164">アイテム作成可能</span><span class="sxs-lookup"><span data-stu-id="a6e03-164">Can create items</span></span>|<span data-ttu-id="a6e03-165">サブ フォルダー作成可能</span><span class="sxs-lookup"><span data-stu-id="a6e03-165">Can create sub folders</span></span>|<span data-ttu-id="a6e03-166">フォルダーの所有者になる</span><span class="sxs-lookup"><span data-stu-id="a6e03-166">Is folder owner</span></span>|<span data-ttu-id="a6e03-167">フォルダーを表示可能</span><span class="sxs-lookup"><span data-stu-id="a6e03-167">Is folder visible</span></span>|<span data-ttu-id="a6e03-168">連絡先フォルダーにする</span><span class="sxs-lookup"><span data-stu-id="a6e03-168">Is folder contact</span></span>|<span data-ttu-id="a6e03-169">アイテムの編集</span><span class="sxs-lookup"><span data-stu-id="a6e03-169">Edit items</span></span>|<span data-ttu-id="a6e03-170">アイテムの削除</span><span class="sxs-lookup"><span data-stu-id="a6e03-170">Delete items</span></span>|<span data-ttu-id="a6e03-171">アイテムの参照可能</span><span class="sxs-lookup"><span data-stu-id="a6e03-171">Can read items</span></span>|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="a6e03-172">None (なし)</span><span class="sxs-lookup"><span data-stu-id="a6e03-172">None</span></span>  <br/> |<span data-ttu-id="a6e03-173">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-173">False</span></span>  <br/> |<span data-ttu-id="a6e03-174">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-174">False</span></span>  <br/> |<span data-ttu-id="a6e03-175">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-175">False</span></span>  <br/> |<span data-ttu-id="a6e03-176">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-176">False</span></span>  <br/> |<span data-ttu-id="a6e03-177">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-177">False</span></span>  <br/> |<span data-ttu-id="a6e03-178">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-178">None</span></span>  <br/> |<span data-ttu-id="a6e03-179">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-179">None</span></span>  <br/> |<span data-ttu-id="a6e03-180">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-180">None</span></span>  <br/> |
|<span data-ttu-id="a6e03-181">Owner</span><span class="sxs-lookup"><span data-stu-id="a6e03-181">Owner</span></span>  <br/> |<span data-ttu-id="a6e03-182">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-182">True</span></span>  <br/> |<span data-ttu-id="a6e03-183">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-183">True</span></span>  <br/> |<span data-ttu-id="a6e03-184">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-184">True</span></span>  <br/> |<span data-ttu-id="a6e03-185">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-185">True</span></span>  <br/> |<span data-ttu-id="a6e03-186">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-186">True</span></span>  <br/> |<span data-ttu-id="a6e03-187">すべて</span><span class="sxs-lookup"><span data-stu-id="a6e03-187">All</span></span>  <br/> |<span data-ttu-id="a6e03-188">すべて</span><span class="sxs-lookup"><span data-stu-id="a6e03-188">All</span></span>  <br/> |<span data-ttu-id="a6e03-189">FullDetails</span><span class="sxs-lookup"><span data-stu-id="a6e03-189">FullDetails</span></span>  <br/> |
|<span data-ttu-id="a6e03-190">PublishingEditor (出版編集者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-190">PublishingEditor</span></span>  <br/> |<span data-ttu-id="a6e03-191">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-191">True</span></span>  <br/> |<span data-ttu-id="a6e03-192">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-192">True</span></span>  <br/> |<span data-ttu-id="a6e03-193">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-193">False</span></span>  <br/> |<span data-ttu-id="a6e03-194">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-194">True</span></span>  <br/> |<span data-ttu-id="a6e03-195">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-195">False</span></span>  <br/> |<span data-ttu-id="a6e03-196">すべて</span><span class="sxs-lookup"><span data-stu-id="a6e03-196">All</span></span>  <br/> |<span data-ttu-id="a6e03-197">すべて</span><span class="sxs-lookup"><span data-stu-id="a6e03-197">All</span></span>  <br/> |<span data-ttu-id="a6e03-198">FullDetails</span><span class="sxs-lookup"><span data-stu-id="a6e03-198">FullDetails</span></span>  <br/> |
|<span data-ttu-id="a6e03-199">Editor (編集者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-199">Editor</span></span>  <br/> |<span data-ttu-id="a6e03-200">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-200">True</span></span>  <br/> |<span data-ttu-id="a6e03-201">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-201">False</span></span>  <br/> |<span data-ttu-id="a6e03-202">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-202">False</span></span>  <br/> |<span data-ttu-id="a6e03-203">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-203">True</span></span>  <br/> |<span data-ttu-id="a6e03-204">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-204">False</span></span>  <br/> |<span data-ttu-id="a6e03-205">すべて</span><span class="sxs-lookup"><span data-stu-id="a6e03-205">All</span></span>  <br/> |<span data-ttu-id="a6e03-206">すべて</span><span class="sxs-lookup"><span data-stu-id="a6e03-206">All</span></span>  <br/> |<span data-ttu-id="a6e03-207">FullDetails</span><span class="sxs-lookup"><span data-stu-id="a6e03-207">FullDetails</span></span>  <br/> |
|<span data-ttu-id="a6e03-208">PublishingAuthor (出版著者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-208">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="a6e03-209">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-209">True</span></span>  <br/> |<span data-ttu-id="a6e03-210">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-210">True</span></span>  <br/> |<span data-ttu-id="a6e03-211">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-211">False</span></span>  <br/> |<span data-ttu-id="a6e03-212">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-212">True</span></span>  <br/> |<span data-ttu-id="a6e03-213">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-213">False</span></span>  <br/> |<span data-ttu-id="a6e03-214">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="a6e03-214">Owned</span></span>  <br/> |<span data-ttu-id="a6e03-215">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="a6e03-215">Owned</span></span>  <br/> |<span data-ttu-id="a6e03-216">FullDetails</span><span class="sxs-lookup"><span data-stu-id="a6e03-216">FullDetails</span></span>  <br/> |
|<span data-ttu-id="a6e03-217">Author (著者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-217">Author</span></span>  <br/> |<span data-ttu-id="a6e03-218">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-218">True</span></span>  <br/> |<span data-ttu-id="a6e03-219">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-219">False</span></span>  <br/> |<span data-ttu-id="a6e03-220">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-220">False</span></span>  <br/> |<span data-ttu-id="a6e03-221">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-221">True</span></span>  <br/> |<span data-ttu-id="a6e03-222">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-222">False</span></span>  <br/> |<span data-ttu-id="a6e03-223">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="a6e03-223">Owned</span></span>  <br/> |<span data-ttu-id="a6e03-224">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="a6e03-224">Owned</span></span>  <br/> |<span data-ttu-id="a6e03-225">FullDetails</span><span class="sxs-lookup"><span data-stu-id="a6e03-225">FullDetails</span></span>  <br/> |
|<span data-ttu-id="a6e03-226">NoneditingAuthor (非編集著者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-226">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="a6e03-227">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-227">True</span></span>  <br/> |<span data-ttu-id="a6e03-228">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-228">False</span></span>  <br/> |<span data-ttu-id="a6e03-229">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-229">False</span></span>  <br/> |<span data-ttu-id="a6e03-230">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-230">True</span></span>  <br/> |<span data-ttu-id="a6e03-231">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-231">False</span></span>  <br/> |<span data-ttu-id="a6e03-232">None (なし)</span><span class="sxs-lookup"><span data-stu-id="a6e03-232">None</span></span>  <br/> |<span data-ttu-id="a6e03-233">Owned (所有)</span><span class="sxs-lookup"><span data-stu-id="a6e03-233">Owned</span></span>  <br/> |<span data-ttu-id="a6e03-234">FullDetails</span><span class="sxs-lookup"><span data-stu-id="a6e03-234">FullDetails</span></span>  <br/> |
|<span data-ttu-id="a6e03-235">Reviewer (校閲者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-235">Reviewer</span></span>  <br/> |<span data-ttu-id="a6e03-236">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-236">False</span></span>  <br/> |<span data-ttu-id="a6e03-237">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-237">False</span></span>  <br/> |<span data-ttu-id="a6e03-238">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-238">False</span></span>  <br/> |<span data-ttu-id="a6e03-239">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-239">True</span></span>  <br/> |<span data-ttu-id="a6e03-240">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-240">False</span></span>  <br/> |<span data-ttu-id="a6e03-241">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-241">None</span></span>  <br/> |<span data-ttu-id="a6e03-242">None (なし)</span><span class="sxs-lookup"><span data-stu-id="a6e03-242">None</span></span>  <br/> |<span data-ttu-id="a6e03-243">FullDetails</span><span class="sxs-lookup"><span data-stu-id="a6e03-243">FullDetails</span></span>  <br/> |
|<span data-ttu-id="a6e03-244">Contributor (投稿者)</span><span class="sxs-lookup"><span data-stu-id="a6e03-244">Contributor</span></span>  <br/> |<span data-ttu-id="a6e03-245">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-245">True</span></span>  <br/> |<span data-ttu-id="a6e03-246">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-246">False</span></span>  <br/> |<span data-ttu-id="a6e03-247">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-247">False</span></span>  <br/> |<span data-ttu-id="a6e03-248">True</span><span class="sxs-lookup"><span data-stu-id="a6e03-248">True</span></span>  <br/> |<span data-ttu-id="a6e03-249">False</span><span class="sxs-lookup"><span data-stu-id="a6e03-249">False</span></span>  <br/> |<span data-ttu-id="a6e03-250">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-250">None</span></span>  <br/> |<span data-ttu-id="a6e03-251">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-251">None</span></span>  <br/> |<span data-ttu-id="a6e03-252">なし</span><span class="sxs-lookup"><span data-stu-id="a6e03-252">None</span></span>  <br/> |
   
<span data-ttu-id="a6e03-253">フォルダー レベルのアクセス許可の要求でカスタム以外のアクセス許可レベルを指定する場合、個別アクセス許可の設定を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a6e03-253">If you specify a non-custom permission level in the folder-level permissions request, you don’t need to specify the individual permission settings. If you do specify an individual permission when you set a permission level, an ErrorInvalidPermissionSettings error will be returned in the response.</span></span> <span data-ttu-id="a6e03-254">アクセス許可レベルを設定する場合、個別アクセス許可を指定すると、応答で **ErrorInvalidPermissionSettings** エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-254">If you specify a non-custom permission level in the folder-level permissions request, you don’t need to specify the individual permission settings. If you do specify an individual permission when you set a permission level, an **ErrorInvalidPermissionSettings** error will be returned in the response.</span></span> 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="a6e03-255">EWS マネージ API を使用してフォルダーのアクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="a6e03-255">Adding folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="a6e03-256"><a name="bk_enableewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a6e03-256"></span></span>

<span data-ttu-id="a6e03-257">次のコード例は、以下の目的で EWS マネージ API を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a6e03-257">The following code example shows how to use the EWS Managed API to:</span></span> 
  
- <span data-ttu-id="a6e03-258">新規ユーザーに対して [FolderPermission](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) オブジェクトを新規作成する。</span><span class="sxs-lookup"><span data-stu-id="a6e03-258">Create a new [FolderPermission](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) object for the new user.</span></span> 
    
- <span data-ttu-id="a6e03-259">[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドを使用して、フォルダーに対する現在のアクセス許可を取得する。</span><span class="sxs-lookup"><span data-stu-id="a6e03-259">Getting the current permissions for a folder by using the [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
    
- <span data-ttu-id="a6e03-260">新しい **FolderPermissions** を [Folder.Permissions](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) プロパティに追加する。</span><span class="sxs-lookup"><span data-stu-id="a6e03-260">Add the new **FolderPermissions** to the [Folder.Permissions](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) property.</span></span> 
    
- <span data-ttu-id="a6e03-261">[Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) メソッドを呼び出して、サーバーに新規アクセス許可を保存する。</span><span class="sxs-lookup"><span data-stu-id="a6e03-261">Call the [Updatehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the new permissions to the server.</span></span> 
    
<span data-ttu-id="a6e03-262">この例では、**service** はメールボックス所有者の有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="a6e03-262">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

<span data-ttu-id="a6e03-263">次のコードの行は、アクセス許可レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-263">The following line of code specifies the permission level.</span></span>
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

<span data-ttu-id="a6e03-264">カスタム アクセス許可レベルを使用する場合は、代わりに次のコードを使用します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-264">If you want to use the custom permission level, use this code instead.</span></span>
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

<span data-ttu-id="a6e03-265">**FolderPermission** オブジェクトをカスタム アクセス許可レベルで作成する場合、書き込み可能な [FolderPermission プロパティ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx)の一部またはすべてを設定できます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-265">You can set any or all of the writable [FolderPermission properties](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) when you create a **FolderPermission** object with a custom permission level.</span></span> <span data-ttu-id="a6e03-266">ただし、アプリケーションが [FolderPermissionLevel](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) を明示的に **Custom** に設定することは決してないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="a6e03-266">Note, however, that the [FolderPermissionLevel](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) is never explicitly set to **Custom** by the application.</span></span> <span data-ttu-id="a6e03-267">**FolderPermission** オブジェクトを作成し、個別アクセス許可を設定する場合のみ、**FolderPermissionLevel** は Custom に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-267">The **FolderPermissionLevel** is set to Custom only when you create a **FolderPermission** object and set individual permissions.</span></span> 
  
## <a name="adding-folder-permissions-by-using-ews"></a><span data-ttu-id="a6e03-268">EWS を使用してフォルダーのアクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="a6e03-268">Adding folder permissions by using EWS</span></span>
<span data-ttu-id="a6e03-269"><a name="bk_enableews"> </a></span><span class="sxs-lookup"><span data-stu-id="a6e03-269"></span></span>

<span data-ttu-id="a6e03-270">次の EWS のコード例では、現在のアクセス許可を取得し、新しいアクセス許可の一覧を送信することによって、特定のフォルダーにアクセス許可を追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a6e03-270">The following EWS code examples show how to add permissions to a specific folder by retrieving the current permissions and then submitting a list of new permissions.</span></span>
  
<span data-ttu-id="a6e03-271">最初の手順は、[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 要求を送信することです。この要求では、[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 値でアクセス許可を追加するフォルダー (この例では [送信済みアイテム] フォルダー) を指定し、[FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 値に folder:PermissionSet を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-271">The first step is to send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request, where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to add permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet. This request will retrieve the permission settings for the folder specified.</span></span> <span data-ttu-id="a6e03-272">この要求は、指定したフォルダーのアクセス許可設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-272">This request will retrieve the permission settings for the folder specified.</span></span> 
  
<span data-ttu-id="a6e03-273">これは、[フォルダーのアクセス許可を追加する](#bk_enableewsma)ために **Bind** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-273">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetFolder>
        <m:FolderShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="a6e03-274">サーバーは、**GetFolder** 要求に [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に取得されたことを示す、値が **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-274">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span> <span data-ttu-id="a6e03-275">[FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 値と [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) 値は、読みやすくするために短縮してあります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-275">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) and [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) values have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="a6e03-276">次に、**UpdateFolder** 操作を使用して、更新された [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) を送信します。それには、新規ユーザーのための [Permission](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6e03-276">Next, use the **UpdateFolder** operation to send the updated [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), which does not include the [Permission](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) for the removed user.</span></span> <span data-ttu-id="a6e03-277">[UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) 操作で各フォルダーの [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) 要素を含めると、そのフォルダーのすべてのアクセス許可設定が上書きされることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a6e03-277">Note that including the [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) element for the respective folder in the [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation will overwrite all the permission settings on the folder.</span></span> <span data-ttu-id="a6e03-278">同様に、**UpdateFolder** 操作の [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) オプションを含めると、フォルダーのすべてのアクセス許可設定が削除されます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-278">Likewise, including the [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) option of the **UpdateFolder** operation will also delete all the permission settings on the folder.</span></span> 
  
<span data-ttu-id="a6e03-279">これは、[フォルダーのアクセス許可を追加する](#bk_enableewsma)ために **Update** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-279">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a6e03-280">次のコードの行は、アクセス許可レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-280">The following line of code specifies the permission level.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="a6e03-281">カスタム アクセス許可レベルを使用する場合は、代わりに次のコードを使用します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-281">If you want to use the custom permission level, use this code instead.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="a6e03-282">サーバーは、**UpdateFolder** 要求に [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に更新されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-282">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully.</span></span>
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="a6e03-283">EWS マネージ API を使用してフォルダーのアクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="a6e03-283">Removing folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="a6e03-284"><a name="bk_removeewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a6e03-284"></span></span>

<span data-ttu-id="a6e03-285">次のコード例は、既定および匿名のアクセス許可を除く、特定のフォルダーのすべてのユーザーのアクセス許可を削除するために、EWS マネージ API を使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a6e03-285">The following code example shows how to use the EWS Managed API to remove all user permissions on a specific folder, except for the default and anonymous permissions, by:</span></span>
  
1. <span data-ttu-id="a6e03-286">**Bind** メソッドを使用して、フォルダーの現在のアクセス許可を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-286">Getting the current permissions for a folder by using the **Bind** method.</span></span> 
    
2. <span data-ttu-id="a6e03-287">**Permissions** コレクションを反復処理し、個別ユーザーのアクセス許可を削除します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-287">Iterating through the **Permissions** collection and removing permissions for individual users.</span></span> 
    
3. <span data-ttu-id="a6e03-288">**Update** メソッドを呼び出して、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-288">Calling the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="a6e03-p114">この例では、フォルダーのすべてのユーザー アクセス許可を削除します。特定のユーザーのアクセス許可のみを削除するようこの例を変更する場合、次のコードの行を変更して、ユーザーの表示名、または SMTP アドレスのいずれかを識別できるようにします。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p114">This example removes all user permissions on a folder. If you want to modify this example to remove permissions only for a specific user, change the following line of code to identify either the display name or SMTP address of the user.</span></span>
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

<span data-ttu-id="a6e03-291">この例では、**service** はメールボックス所有者の有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="a6e03-291">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a><span data-ttu-id="a6e03-292">EWS を使用してフォルダーのアクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="a6e03-292">Removing folder permissions by using EWS</span></span>
<span data-ttu-id="a6e03-293"><a name="bk_removeews"> </a></span><span class="sxs-lookup"><span data-stu-id="a6e03-293"></span></span>

<span data-ttu-id="a6e03-294">EWS の次のコード例は、既定および匿名のアクセス許可を除く、特定のフォルダーのすべてのユーザーのアクセス許可を削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-294">The following EWS code examples show how to remove all user permissions on a specific folder, except for the default and anonymous permissions.</span></span>
  
<span data-ttu-id="a6e03-295">最初の手順は、[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 要求を送信することです。この要求では、[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 値でアクセス許可を削除するフォルダー (この例では [送信済みアイテム] フォルダー) を指定し、[FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 値に folder:PermissionSet を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-295">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to remove permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet. This request will retrieve the PermissionSet for the folder specified.</span></span> <span data-ttu-id="a6e03-296">この要求は、指定したフォルダーの [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-296">This request will retrieve the [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) for the folder specified.</span></span> 
  
<span data-ttu-id="a6e03-297">これは、[フォルダーのアクセス許可を削除する](#bk_removeewsma)ために **Bind** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-297">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a6e03-298">サーバーは、**GetFolder** 要求に [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に取得されたことを示す、値が **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-298">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span> <span data-ttu-id="a6e03-299">**FolderId** 要素の値と **ParentFolderId** 要素の値は、読みやすくするために短縮してあります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-299">The values of the **ItemId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="a6e03-300">次に、**UpdateFolder** 操作を使用し、更新された **PermissionSet** を送信します。削除したユーザーの **Permission** は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="a6e03-300">Next, use the **UpdateFolder** operation to send the updated **PermissionSet**, which does not include the **Permission** for the removed user.</span></span> 
  
<span data-ttu-id="a6e03-301">これは、[フォルダーのアクセス許可を削除する](#bk_removeewsma)ために **Update** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-301">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a6e03-302">サーバーは、**UpdateFolderResponse** メッセージで **UpdateFolder** 要求に応答します。このメッセージには、更新が正常に完了したことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a6e03-302">The server responds to the **UpdateFolder** request with an **UpdateFolderResponse** message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="a6e03-303">EWS マネージ API を使用してフォルダーのアクセス許可を更新する</span><span class="sxs-lookup"><span data-stu-id="a6e03-303">Updating folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="a6e03-304"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a6e03-304"></span></span>

<span data-ttu-id="a6e03-p117">EWS マネージ API を使用して、特定のフォルダーのフォルダーのアクセス許可を更新することもできます。アクセス許可を更新するには、次のことを行います。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p117">You can also update folder permissions for a specific folder by using the EWS Managed API. To update the permissions:</span></span> 
  
1. <span data-ttu-id="a6e03-307">古いアクセス許可の[フォルダーのアクセス許可を削除します](#bk_removeewsma)が、(まだ) **Update** メソッドを呼び出しません。</span><span class="sxs-lookup"><span data-stu-id="a6e03-307">[Remove the folder permissions](#bk_removeewsma) for the outdated permissions, but do not call the **Update** method (yet).</span></span> 
    
2. <span data-ttu-id="a6e03-308">[新規または変更されたユーザーのフォルダーのアクセス許可を追加します](#bk_enableewsma)。</span><span class="sxs-lookup"><span data-stu-id="a6e03-308">[Add folder permissions for the new or changed users](#bk_enableewsma).</span></span>
    
3. <span data-ttu-id="a6e03-309">**Update** メソッドを呼び出して、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-309">Call the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="a6e03-310">同じユーザーのアクセス許可の 2 つのセットを追加しようとする場合、「指定したアクセス許可のセットには、重複したユーザー Id が含まれています」という説明がある **ServiceResponseException** エラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-310">If you try to add two sets of permissions for the same user, you will receive a **ServiceResponseException** error with the following description: "The specified permission set contains duplicate UserIds". In that case, remove the current permissions from the Permission collection, then add the new permissions to the Permission collection.</span></span> <span data-ttu-id="a6e03-311">このケースでは、**Permission** コレクションから現在のアクセス許可を削除してから、新しいアクセス許可を **Permission** コレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-311">In that case, remove the current permissions from the **Permission** collection, then add the new permissions to the **Permission** collection.</span></span> 
  
## <a name="updating-folder-permissions-by-using-ews"></a><span data-ttu-id="a6e03-312">EWS を使用してフォルダーのアクセス許可を更新する</span><span class="sxs-lookup"><span data-stu-id="a6e03-312">Updating folder permissions by using EWS</span></span>
<span data-ttu-id="a6e03-313"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="a6e03-313"></span></span>

<span data-ttu-id="a6e03-p119">EWS を使用して、削除と追加のプロセスを組み合わせ、特定のフォルダーのフォルダーのアクセス許可を更新することもできます。アクセス許可を更新するには、次のことを行います。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p119">You can also update folder permissions for specific folders by using EWS by combining the removal and addition process. To update the permissions:</span></span> 
  
1. <span data-ttu-id="a6e03-316">**GetFolder** 操作を使用して、フォルダーの現在のアクセス許可を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-316">Retrieve the folder's current permissions by using the **GetFolder** operation.</span></span> 
    
2. <span data-ttu-id="a6e03-317">**UpdateFolder** 操作を使用して、更新されたアクセス許可の一覧を送信します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-317">Send an updated list of permissions by using the **UpdateFolder** operation.</span></span> 
    
<span data-ttu-id="a6e03-318">これらは、EWS を使用して[アクセスの有効化](#bk_enableews)または[アクセスの削除](#bk_removeews)を行うのに使用するのと同じ 2 つの操作です。</span><span class="sxs-lookup"><span data-stu-id="a6e03-318">These are the same two operations you use to [enable](#bk_enableews) or [remove access](#bk_removeews) by using EWS.</span></span> <span data-ttu-id="a6e03-319">唯一の違いは、**GetFolder** 応答を受信したときにユーザーの **Permission** 設定が含まれていることです。</span><span class="sxs-lookup"><span data-stu-id="a6e03-319">The only difference is that when you receive the **GetFolder** response, it will contain a **Permission** set for user.</span></span> <span data-ttu-id="a6e03-320">単に既存の **Permission** 要素を新しい **Permission** 要素に取り替え、新しい **Permission** の値 (複数の場合もある) を指定して **UpdateFolder** 操作を送信します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-320">Simply replace that existing **Permission** element with the new **Permission** element, and then send the **UpdateFolder** operation with the new **Permission** value or values.</span></span> 
  
<span data-ttu-id="a6e03-321">同じユーザーに、アクセス許可のセットを 2 つ追加しようとすると、値が **ErrorDuplicateUserIdsSpecified** の **ResponseCode** を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="a6e03-321">If you try to add two sets of permissions for the same user, you will receive a ResponseCode value of ErrorDuplicateUserIdsSpecified. In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span> <span data-ttu-id="a6e03-322">このケースでは、要求からユーザーのアクセス許可の古い値を削除してから、要求を再試行します。</span><span class="sxs-lookup"><span data-stu-id="a6e03-322">If you try to add two sets of permissions for the same user, you will receive a ResponseCode value of ErrorDuplicateUserIdsSpecified. In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a6e03-323">次の手順</span><span class="sxs-lookup"><span data-stu-id="a6e03-323">Next steps</span></span>

<span data-ttu-id="a6e03-p122">ユーザーのアクセス許可を特定のフォルダーに設定した後、そのユーザーは代理人としてフォルダーにアクセスできます。詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6e03-p122">After you give a user permission to a specific folder, the user can access the folder as a delegate. For more information, see:</span></span>
  
- [<span data-ttu-id="a6e03-326">Exchange で EWS を使用して、代理人としてメールにアクセスする</span><span class="sxs-lookup"><span data-stu-id="a6e03-326">How to: Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a6e03-327">Exchange で EWS を使用して予定表に代理人としてアクセスする</span><span class="sxs-lookup"><span data-stu-id="a6e03-327">How to: Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a6e03-328">Exchange で EWS を使用して、代理人として連絡先にアクセスする</span><span class="sxs-lookup"><span data-stu-id="a6e03-328">How to: Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="a6e03-329">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6e03-329">See also</span></span>

- [<span data-ttu-id="a6e03-330">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="a6e03-330">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="a6e03-331">Exchange で EWS を使用して代理人を追加および削除する</span><span class="sxs-lookup"><span data-stu-id="a6e03-331">How to: Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="a6e03-332">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="a6e03-332">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

