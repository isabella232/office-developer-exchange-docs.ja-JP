---
title: Exchange での受信トレイの管理と EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3dfa0fc9-64bb-4d18-bff7-bf6b3bed4a0d
description: 受信トレイのルールと受信拒否リストを使用して、EWS Mマネージ API または EWS アプリケーションで受信トレイを管理する方法を紹介します。
ms.openlocfilehash: 7c88015386dc882f14184765e0046a866e8c0e10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456317"
---
# <a name="inbox-management-and-ews-in-exchange"></a><span data-ttu-id="1b7fb-103">Exchange での受信トレイの管理と EWS</span><span class="sxs-lookup"><span data-stu-id="1b7fb-103">Inbox management and EWS in Exchange</span></span>

<span data-ttu-id="1b7fb-104">受信トレイのルールと受信拒否リストを使用して、EWS Mマネージ API または EWS アプリケーションで受信トレイを管理する方法を紹介します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-104">Find out how you can manage your Inbox in your EWS Managed API or EWS application by using Inbox rules and the blocked senders list.</span></span>
  
<span data-ttu-id="1b7fb-p101">Exchange メールボックスには、ユーザーが受信メールを自動的に整理できるようになる機能が備わっています。これらの機能はすべて、ユーザーによる操作なしでサーバー上で動作しますが、さまざまなニーズに対応できます。EWS マネージ API と EWS では、これらの機能へのアクセスが提供され、ユーザーは自分の受信トレイを管理できるようになります。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p101">Exchange mailboxes come equipped with features to help users organize their incoming mail automatically. These features all operate on the server without user intervention, but they serve different needs. The EWS Managed API and EWS provide access to these features, enabling your users to manage their Inboxes.</span></span>
  
<span data-ttu-id="1b7fb-108">**表 1. 受信トレイの管理機能**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-108">**Table 1. Inbox management features**</span></span>

|<span data-ttu-id="1b7fb-109">**目的…**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-109">**If you want to…**</span></span>|<span data-ttu-id="1b7fb-110">**使う機能**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-110">**Use…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b7fb-111">特定の条件 (送信者、件名、添付物など) に基づいて、受信メッセージにアクション (別のフォルダーへの移動、削除など) を行う</span><span class="sxs-lookup"><span data-stu-id="1b7fb-111">Take action on incoming messages (such as moving them to another folder or deleting them) based on specific criteria (such as sender, subject, or attachments)</span></span>  <br/> |<span data-ttu-id="1b7fb-112">受信トレイのルール</span><span class="sxs-lookup"><span data-stu-id="1b7fb-112">Inbox rules</span></span>  <br/> |
|<span data-ttu-id="1b7fb-113">特定の送信者からのすべての受信メールを削除する</span><span class="sxs-lookup"><span data-stu-id="1b7fb-113">Delete all incoming mail from a particular sender</span></span>  <br/> |<span data-ttu-id="1b7fb-114">受信拒否リスト</span><span class="sxs-lookup"><span data-stu-id="1b7fb-114">Blocked Senders List</span></span>  <br/> |
   
## <a name="inbox-rules"></a><span data-ttu-id="1b7fb-115">受信トレイ ルール</span><span class="sxs-lookup"><span data-stu-id="1b7fb-115">Inbox rules</span></span>
<span data-ttu-id="1b7fb-116"><a name="bk_InboxRules"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-116"><a name="bk_InboxRules"> </a></span></span>

<span data-ttu-id="1b7fb-p102">現実問題: すべてのメールが同じように作成されているわけではありません。数年前に参加し、なかなか退会する機会がなかったインターネットのねこ動画の配布リストからのメールが、自分の上司から受け取るメールと同じ数ほどあるとします。インターネットのねこ動画は面白いですが、配布リストからのメールに使用されるトラフィック量は大きいですし、配布リストからのメールが受信トレイに大量に来るため重要なメッセージを簡単に見失ってしまう恐れがあります。多くのユーザーは、受信トレイ ルールを使用してそのようなメッセージを減らし、受信トレイをはるかに使いやすい場所にします。Exchange Web サービス (EWS) を使用すれば、アプリケーションは、制限ルールの機能を有効に活用できます。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p102">Let's face it: not every email message is created equal. For every email a user gets from his or her manager, there's one from an Internet cat video distribution list he or she joined years ago and never got around to leaving. While Internet cat videos are entertaining, the amount of traffic that distribution list gets can get out of hand, and important messages can easily be lost in the sea of distribution list mail in an Inbox. Many users turn to Inbox rules to help pare down those messages, and make their Inbox a much nicer place to be. With Exchange Web Services (EWS), your application can bring the power of rules to bear.</span></span>
  
<span data-ttu-id="1b7fb-p103">EWS マネージ API では、ルールを操作するために [ExchangeService.GetInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) メソッドと [ExchangeService.UpdateInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) メソッドが提供されます。EWS では、ルールを操作するために [GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) 操作と [UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) 操作が提供されます。ただし、EWS マネージ API と EWS には、受信トレイ ルールを操作する場合、次の制限があることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p103">The EWS Managed API provides the [ExchangeService.GetInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) and [ExchangeService.UpdateInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) methods for working with rules. EWS provides the [GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) and [UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) operations for working with rules. However, note that the EWS Managed API and EWS have the following limitations when working with Inbox rules:</span></span> 
  
- <span data-ttu-id="1b7fb-125">EWS では、"クライアントのみ" ルール、または Outlook で設定されている "このコンピューターでのみ" 実行されるルールにアクセスしたり、作成したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-125">EWS cannot access or create "client-only" rules or rules that are set in Outlook to run "on this computer only".</span></span>
    
- <span data-ttu-id="1b7fb-p104">EWS を使用して現在の一連のルールを変更するには、Outlook ルールの BLOB が存在する場合、これを削除する必要があります。これは、ルールの変更に EWS を使用すると、Outlook によって既にオフ (無効) にされていたすべてのルールが削除されることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p104">To change the current set of rules by using EWS, you have to remove the Outlook rules BLOB, if it is present. This means that using EWS to modify rules deletes any rules that were previously turned off (disabled) by using Outlook.</span></span> 
    
### <a name="how-do-rules-work"></a><span data-ttu-id="1b7fb-128">ルールのしくみ</span><span class="sxs-lookup"><span data-stu-id="1b7fb-128">How do rules work?</span></span>
<span data-ttu-id="1b7fb-129"><a name="bk_HowRulesWork"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-129"><a name="bk_HowRulesWork"> </a></span></span>

<span data-ttu-id="1b7fb-p105">ルール エンジンは、ユーザーのメールボックスに対するゲートキーパーとして機能します。ユーザーのメールボックスにメッセージが到着すると、受信トレイにメッセージが表示される前に、そのメッセージは、ルールの順序付きリストに対して評価されます。これは、到着時のみに受信トレイでのみ実行されることにご注意ください。これらのルールは、[条件](#bk_Conditions)、[アクション](#bk_Actions)、[例外](#bk_Exceptions)の 3 つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p105">The rules engine acts as a gatekeeper to a user's mailbox. As a message arrives in the user's mailbox, but before the message appears in the Inbox, that message is evaluated against an ordered list of rules. Note that this only occurs at arrival time, and only in the Inbox. These rules are comprised of three parts: [Conditions](#bk_Conditions), [Actions](#bk_Actions), and [Exceptions](#bk_Exceptions).</span></span>
  
<span data-ttu-id="1b7fb-134">ルール エンジンは、ルールの一覧の最上位のルールから開始して、最後のルールに到達するまで次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-134">Starting with the rule at the top of the rule list, the rules engine performs the following steps until it reaches the end of the list of rules:</span></span>
  
1. <span data-ttu-id="1b7fb-135">ルールで指定されたすべての条件を満しているかどうかメッセージを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-135">Checks the message to determine whether it meets all the conditions specified in the rule.</span></span>
    
1. <span data-ttu-id="1b7fb-136">メッセージがすべての条件を満たしている場合、手順 2 で評価を続行します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-136">If it meets all the conditions, evaluation continues with step 2.</span></span>
    
2. <span data-ttu-id="1b7fb-137">そうでない場合は、ルール エンジンはルール一覧の次のルールを読み込み、手順 1 からやり直します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-137">If it does not meet all the conditions, the rules engine loads the next rule in the rule list and starts over at step 1.</span></span>
    
2. <span data-ttu-id="1b7fb-138">ルールで指定されたいずれかの例外を満しているかどうかメッセージを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-138">Checks the message to determine whether it meets any of the exceptions specified in the rule.</span></span>
    
1. <span data-ttu-id="1b7fb-139">メッセージがいずれかの例外を満たしている場合、ルール エンジンはルール一覧の次のルールを読み込み、手順 1 からやり直します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-139">If it meets any of the exceptions, the rules engine loads the next rule in the rule list and starts over at step 1.</span></span>
    
2. <span data-ttu-id="1b7fb-140">そうでない場合は、手順 3 で評価が続行されます。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-140">If it does not meet any of the exceptions, evaluation continues with step 3.</span></span>
    
3. <span data-ttu-id="1b7fb-141">ルールで指定されたアクションをメッセージに実行します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-141">Performs the actions specified in the rule on the message.</span></span>
    
1. <span data-ttu-id="1b7fb-142">"以降のルールは処理しない" アクションが指定されると、ルール エンジンはその他のすべてのアクションをメッセージに実行し、メッセージに対するそれ以上のルール評価を行わずに終了します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-142">If the "stop processing more rules" action is specified, the rules engine performs all the other actions on the message, then exits without evaluating any additional rules against the message.</span></span>
    
2. <span data-ttu-id="1b7fb-143">"以降のルールは処理しない" アクションを指定しない場合は、ルール エンジンはルール一覧の次のルールを読み込み、手順 1 からやり直します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-143">If the "stop processing more rules" action is not specified, the rules engine loads the next rule in the rule list and starts over at step 1.</span></span>
    
<span data-ttu-id="1b7fb-144">ルール エンジンが実行するプロセスを次の図に示します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-144">The following figure shows the process that the rules engine follows.</span></span>
  
<span data-ttu-id="1b7fb-145">**図 1.ルール エンジンの概要**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-145">**Figure 1: Rules engine overview**</span></span>

![図はルール エンジンが使用する手順を示しており、ルールの評価から始まり、ルールの条件が満たされたかどうかを判断して、アクションを実行するか、または終了するまで次のルールへ移行します。](media/Ex15_Rules_EngineOverview.png)
  
### <a name="putting-the-pieces-together---parts-of-a-rule"></a><span data-ttu-id="1b7fb-147">ルールの構成要素を理解する</span><span class="sxs-lookup"><span data-stu-id="1b7fb-147">Putting the pieces together - parts of a rule</span></span>
<span data-ttu-id="1b7fb-148"><a name="bk_Pieces"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-148"><a name="bk_Pieces"> </a></span></span>

<span data-ttu-id="1b7fb-149">ルールの各部を視覚化する方法の1つは、受信メールを整理する必要があるユーザーに指示を与えることを想像することです。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-149">One way to visualize the parts of a rule is to imagine that you are giving instructions to someone who is tasked with organizing your incoming email.</span></span> <span data-ttu-id="1b7fb-150">この人物には、「メッセージが到着した場合はメッセージを受信しない」と言うことがあります。 \<insert conditions here\> \<insert actions here\> \<insert exceptions here\></span><span class="sxs-lookup"><span data-stu-id="1b7fb-150">You might say to this person: "When a message arrives that \<insert conditions here\>, do \<insert actions here\>, unless the message \<insert exceptions here\>.</span></span> <span data-ttu-id="1b7fb-151">各パーツを詳しく見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-151">Let's take a closer look at each part.</span></span>
  
#### <a name="conditions"></a><span data-ttu-id="1b7fb-152">条件</span><span class="sxs-lookup"><span data-stu-id="1b7fb-152">Conditions</span></span>
<span data-ttu-id="1b7fb-153"><a name="bk_Conditions"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-153"><a name="bk_Conditions"> </a></span></span>

<span data-ttu-id="1b7fb-p107">[条件](https://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) は、ルールを適用する場合について説明します。ルールの条件は省略できます (ルールがすべての受信メッセージに適用されます) が、普通は受信メッセージのサブセットに適用される条件をルールに設定します。たとえば、"メッセージが Sadie からの場合" または "メッセージが 'ねこ動画の愛好家' の配布リストに送信される場合" などです。ルールには複数の条件を指定することができます。ルールに複数の条件がある場合、ルール エンジンが指定されたアクションを実行するためには、すべての条件が満たされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p107">[Conditions](https://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) describe when a rule should be applied. While you can omit the conditions of a rule (resulting in a rule that applies to every message received), it is far more common for rules to have conditions that apply to a subset of incoming messages. Some examples are "when a message is from Sadie" or "when a message is sent to the 'Cat Video Lovers' distribution list". Rules can have multiple conditions. When rules have more than one condition, all the conditions must be met in order for the rules engine to take the specified action.</span></span> 
  
#### <a name="actions"></a><span data-ttu-id="1b7fb-159">アクション</span><span class="sxs-lookup"><span data-stu-id="1b7fb-159">Actions</span></span>
<span data-ttu-id="1b7fb-160"><a name="bk_Actions"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-160"><a name="bk_Actions"> </a></span></span>

<span data-ttu-id="1b7fb-p108">[Actions](https://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) describe what happens when a rule applies. Examples are "move the message to the 'Cats' folder" or "mark the message with 'Low' importance". Rules can have multiple actions. When you specify multiple actions for a rule, all the actions are performed when the rule is applied.</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p108">[Actions](https://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) describe what happens when a rule applies. Examples are "move the message to the 'Cats' folder" or "mark the message with 'Low' importance". Rules can have multiple actions. When you specify multiple actions for a rule, all the actions are performed when the rule is applied.</span></span> 
  
#### <a name="exceptions"></a><span data-ttu-id="1b7fb-165">例外</span><span class="sxs-lookup"><span data-stu-id="1b7fb-165">Exceptions</span></span>
<span data-ttu-id="1b7fb-166"><a name="bk_Exceptions"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-166"><a name="bk_Exceptions"> </a></span></span>

<span data-ttu-id="1b7fb-p109">例</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p109">[Exceptions](https://msdn.microsoft.com/library/7cd63ac2-3441-4ed4-915b-6f90af4b28fc%28Office.15%29.aspx) describe when a rule should not apply, even if the criteria specified in the conditions are met. Examples are "except if the message is sent only to me" or "except if the message is from Mom". A rule can have multiple exceptions. When rules have more than one exception, and any of the exceptions are met, the rule is not applied.</span></span> 
  
### <a name="example-herding-those-cats"></a><span data-ttu-id="1b7fb-171">例:これらのねこ動画を寄せ集める</span><span class="sxs-lookup"><span data-stu-id="1b7fb-171">Example: Herding those cats</span></span>
<span data-ttu-id="1b7fb-172"><a name="bk_Example"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-172"><a name="bk_Example"> </a></span></span>

<span data-ttu-id="1b7fb-p110">ルールを使用してインターネットのねこ動画の配信リストからのトラフィックを削除する方法を見てみましょう。前提条件は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p110">Let's take a look at how your users can use rules to eliminate the traffic from that Internet cat video distribution list. Let's assume the following:</span></span>
  
- <span data-ttu-id="1b7fb-175">これらのメッセージは、"インターネットのねこ動画愛好家" という配布リストに送信されます。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-175">These messages are sent to a distribution list called "Internet Cat Video Enthusiasts".</span></span>
    
- <span data-ttu-id="1b7fb-p111">そのうちこれらのメッセージは読みたいのですが、自分の受信トレイをこれらのメッセージで散らかった状態にしたくはありません。これらのメッセージを "ねこ" というフォルダーに置きたいと考えています。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p111">Your users want to read these messages eventually, they just don't want them cluttering their Inbox. They'd rather file them in a folder called "Cats".</span></span>
    
- <span data-ttu-id="1b7fb-178">母親 が一番面白いビデオを送信してくるので、母親がこの配布リストに送信したメッセージはすぐに読みたいと思っています。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-178">Your users want to read messages sent to this distribution list by their mother right away, because Mom sends the funniest videos.</span></span>
    
<span data-ttu-id="1b7fb-179">このためには、次のようにルール エンジンに指定します。"'インターネットのねこ動画愛好家' 配布リストに送信されるメッセージを受け取ったら、そのメッセージが 母親 からのものではない限り、'ねこ' フォルダーに移動します。"</span><span class="sxs-lookup"><span data-stu-id="1b7fb-179">This tells the rules engine the following: "When a message arrives that is sent to the 'Internet Cat Video Enthusiasts' distribution list, move it to the 'Cats' folder, unless the message is from Mom."</span></span> 
  
<span data-ttu-id="1b7fb-180">**表 2. ルールの定義**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-180">**Table 2. Rule definition**</span></span>

|<span data-ttu-id="1b7fb-181">**ルールの構成要素**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-181">**Rule part**</span></span>|<span data-ttu-id="1b7fb-182">**値**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-182">**Value**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b7fb-183">条件</span><span class="sxs-lookup"><span data-stu-id="1b7fb-183">Conditions</span></span>  <br/> |<span data-ttu-id="1b7fb-184">'インターネットのねこ動画愛好家' 配布リストに送信される</span><span class="sxs-lookup"><span data-stu-id="1b7fb-184">Sent to the 'Internet Cat Video Enthusiasts' distribution list</span></span>  <br/> |
|<span data-ttu-id="1b7fb-185">アクション</span><span class="sxs-lookup"><span data-stu-id="1b7fb-185">Actions</span></span>  <br/> |<span data-ttu-id="1b7fb-186">メッセージを'ねこ' フォルダーに移動する、</span><span class="sxs-lookup"><span data-stu-id="1b7fb-186">Move the message to the 'Cats' folder</span></span>  <br/> <span data-ttu-id="1b7fb-187">かつ、以降のルールは処理しない</span><span class="sxs-lookup"><span data-stu-id="1b7fb-187">AND stop processing more rules</span></span>  <br/> |
|<span data-ttu-id="1b7fb-188">Exceptions</span><span class="sxs-lookup"><span data-stu-id="1b7fb-188">Exceptions</span></span>  <br/> |<span data-ttu-id="1b7fb-189">'母親' から</span><span class="sxs-lookup"><span data-stu-id="1b7fb-189">From 'Mom'</span></span>  <br/> |
   
> [!NOTE]
> <span data-ttu-id="1b7fb-p112">"以降のルールは処理しない" は、該当したルールのアクションの 1 つであることに注意してください。通常、どのルールが特定のメッセージで機能するかについての混乱を避けるため、このアクションを含めることをお勧めします。ただし、このアクションを省略しルールを適切に順序付ければ、受信メールのより高度な処理を実行できます。この場合、おそらく、インターネットのねこ動画 メッセージでは、高度な処理をあまり行わないことが安全策です。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p112">Notice that "stop processing more rules" is one of the actions in the resulting rule. In general it's a good idea to include this action to avoid confusion over which rules act on any given message. However, by omitting this action and properly ordering your rules, you can achieve more advanced processing of your incoming mail. In this case, it's probably a safe bet that Internet cat video messages don't require much in the way of advanced processing.</span></span> 
  
<span data-ttu-id="1b7fb-p113">このルールの作成後、すぐに新しいメッセージが届きました。同僚の Hope が配布リストにメッセージを送信しました。ルール エンジンの機能を頭の中で実行してみると、メッセージがすべての条件を満たし ('インターネットのねこ動画愛好家' に送られ)、かつ例外のいずれも満たさない ('母親' から送信されていない) と、ルールが適用され、メッセージは 'ねこ' フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p113">Shortly after creating this rule, a new message comes in. A coworker Hope sends a message to the distribution list. If we mentally perform the work of the rules engine, the message meets all the conditions (it is sent to 'Internet Cat Videos Enthusiasts'), and it meets none of the exceptions (it isn't from 'Mom'), so the rule applies and the message gets moved to the 'Cats' folder.</span></span>
  
<span data-ttu-id="1b7fb-197">次の図は、受信メッセージにルールを適用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-197">The following figure shows how the rule is applied to an incoming mail message.</span></span>
  
<span data-ttu-id="1b7fb-198">**図 2. 受信メッセージがルールによって処理されます。**</span><span class="sxs-lookup"><span data-stu-id="1b7fb-198">**Figure 2. Incoming message is processed by a rule**</span></span>

![図は新しいメッセージが同僚の配布リストに送信されることを示しています。メッセージはすべての条件を満たしており、ルールで定義されたどの例外にも該当しないため、猫のフォルダーに移動されます。](media/Ex15_Rules_RuleEvaluationSample.png)
  
## <a name="blocking-senders"></a><span data-ttu-id="1b7fb-201">送信者をブロックする</span><span class="sxs-lookup"><span data-stu-id="1b7fb-201">Blocking senders</span></span>
<span data-ttu-id="1b7fb-202"><a name="bk_Blocking"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-202"><a name="bk_Blocking"> </a></span></span>

<span data-ttu-id="1b7fb-p115">特定の送信者からのすべてのメールを迷惑メール フォルダーに移動するルールを作成できますが、これは迷惑メールのオプションで受信拒否リストを使用して行うこともできます。ユーザーが指定できるルールの数には制限があるため、受信拒否リストを使用するのが有効な方法です。[ExchangeService.MarkAsJunk](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) EWS マネージ API メソッドまたは [MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS 操作を使用して、 [受信拒否リストに対して特定のメール アドレスを追加または削除](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)できます。EWS が受信拒否リストにアクセスするためには、ユーザーのメールボックスに、追加または削除するメール アドレスからのメール メッセージを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b7fb-p115">Although you can create a rule that will move all mail from a specific sender to the Junk Mail folder, you can also do this by using the Blocked Senders List in your Junk Email options. Because there is a limit to how many rules a user can have, it makes sense to use the Blocked Senders List. You can [add or remove specific email addresses from the Blocked Senders List](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) by using the [ExchangeService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API method or the [MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) EWS operation. Note that in order for EWS to access the Blocked Senders List, the user's mailbox must contain an email message from the email address that you want to add or remove.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="1b7fb-207">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="1b7fb-207">In this section</span></span>
<span data-ttu-id="1b7fb-208"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7fb-208"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="1b7fb-209">Exchange で EWS を使用して受信トレイ ルールを管理する</span><span class="sxs-lookup"><span data-stu-id="1b7fb-209">Manage Inbox rules by using EWS in Exchange</span></span>](how-to-manage-inbox-rules-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="1b7fb-210">Exchange で EWS を使用して、受信拒否リストに対してメール アドレスを追加、削除する</span><span class="sxs-lookup"><span data-stu-id="1b7fb-210">Add and remove email addresses from the Blocked Senders List by using EWS in Exchange</span></span>](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md)
    
## <a name="see-also"></a><span data-ttu-id="1b7fb-211">関連項目</span><span class="sxs-lookup"><span data-stu-id="1b7fb-211">See also</span></span>


- [<span data-ttu-id="1b7fb-212">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="1b7fb-212">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="1b7fb-213">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="1b7fb-213">GetInboxRules operation</span></span>](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [<span data-ttu-id="1b7fb-214">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="1b7fb-214">UpdateInboxRules operation</span></span>](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    
- <span data-ttu-id="1b7fb-215">
  [MarkAsJunk 操作](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1b7fb-215">[MarkAsJunk operation](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)</span></span>
    

