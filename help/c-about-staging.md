---
description: ステージングを使用すると、ライブインデックスに影響を与えることなく、設定や設定に対する変更をテストおよびプレビューできます。
seo-description: ステージングを使用すると、ライブインデックスに影響を与えることなく、設定や設定に対する変更をテストおよびプレビューできます。
seo-title: ステージングについて
solution: Target
title: ステージングについて
topic: Staging,Site search and merchandising
uuid: 2e5889a6-2e9c-4ac7-9d6e-d35e7cafda5b
translation-type: tm+mt
source-git-commit: ef818327e1cdaad79ac47575a8dfba1de3dc5c2e

---


# ステージングについて{#about-staging}

ステージングを使用すると、ライブインデックスに影響を与えることなく、設定や設定に対する変更をテストおよびプレビューできます。

## ステージングについて {#concept_08B8F3CA1F4241108F14BA7FC7806CA7}

ステージングを使用すると、ライブインデックスに影響を与えることなく、設定や設定に対する変更をテストおよびプレビューできます。

要素 [ID:context_A5783D07C72042EC8886F300FFF62C50も参照してください](c-about-simulator.md#context_A5783D07C72042EC8886F300FFF62C50)。

ステージングオプションを持つ任意のページ、ま **[!UICONTROL Push All Live]** たはそ **[!UICONTROL View Live Settings]** のページのすべての設定をステージングできることを意味するページ。 ただし、IndexのWebページは例外です。 この領域のページは、ステージングされたインデックスまたはライブインデックスに対して明示的に作成され、2つのインデックスを個別に直接制御できます。

インデックスを含め、ほとんどすべてのステージを作成できます。 例外には、ステージング環境と実稼働環境の両方に同時に影響を与えるアカウント固有の設定や、インデックス作成操作のスケジュール設定などがあります。 デフォルトでは、ステージング可能な設定に対する変更を保存すると、自動的にステージングされます。

またはオプ **[!UICONTROL Push All Live]** ションが有 **[!UICONTROL View Lives Settings]** 効（グレー表示）でない場合は、そのページのステージ設定がライブ設定と同じであることを意味します。

ステージングされたアイテムの場合、設定のライブバージョンは読み取り専用です。ステージ設定をライブにプッシュすることでのみ操作できます。

## ステージページの履歴について {#section_5BE780AFF26A450A9EFF4000DE53531B}

ほとんどのステージ設定で [!DNL History] は、ページの右上の領域にオプションがあります。 をクリックす **[!UICONTROL History]**&#x200B;ると、開いている特定のステージページに対して最近行った変更を元に戻すことができます。

また、変更ログを表示して、履歴の別の表示を確認することもできます。 変更が適用されるたびに、基になるデータファイルのバックアップバージョンが作成されます。 変更ログには、該当する各リビジョン、バージョン番号、変更を実行したユーザの電子メールアドレス、バックアップが行われた日付が表示されます。 太字のバージョン値を持つエントリは、現在のバージョンを表します。

See [Viewing the Change Log](c-about-reports-menu/c-about-reports-menu.md#task_166F1156719F4B3D834BEA8E249C8057).

## ステージライブ設定の管理ページ {#section_E72B8CAF516345A5B6B6783CF6E512EE}

特定のページ内 **[!UICONTROL Push All Live]** から直接お **[!UICONTROL View Live Settings]** よびオプションを提供する以外に、ページを使用して同 **[!UICONTROL Manage Stage-Live Settings]** 様の操作を行うこともできます。 メイン **[!UICONTROL Manage Stage-Live Settings]** 製品メニューから利用できるページは、現在ステージングされているアカウント内のすべての設定を一元的に表示する場所です。 すべての設定をライブにプッシュ、選択した設定のみをライブにプッシュ、または設定を削除できます。 ただし、ベストプラクティスとして、相互依存の問題を避けるために、すべてのステージングされたアイテムを常にライブにプッシュします。

ページ上の設定は、カテゴリ別にグループ化されます。 各カテゴリを展開して、どのページの設定がステージングされているかを表示できます。 現在、依存関係はステージマネージャー内で追跡されません。 したがって、インデックスを除くすべての項目を一度にライブにすることをお勧めします。

ステージングされたインデックスをライブにプッシュできます。 最初に、ステージングされたインデックスが古いか破損していないことを確認してください。 誤ってステージングされたインデックスをライブにプッシュした場合は、古いライブインデックスをロールバックできます。 ステージングされたインデックスをライブにプッシュするのに通常30秒未満かかります。

## ステージ設定またはインデックスのテスト {#section_6800E52D20854A779946EAB600801F12}

テストコントロールをサポートするページでは、ステージング設定またはライブ設定に対してテストを実行できます。 ステージ設定を表示すると、そのステージ設定がテストに使用されます。 同様に、ライブ設定を表示している場合、テストではライブ設定が使用されます。 テンプレートセクションでは、すべてのテストはインデックスのステージングされたバージョンに対して行われます。 ステージインデックスを検索するには、 `sp_staged` CGIパラメータを1に設定します。 これは、ステージングされたインデックスを使用することを示します。 ステージングされたインデックスが存在しない場合は、ライブインデックスが検索され、必要に応じてステージングされた検索時の設定が適用されます。

バックエンド検索 [CGIパラメーターも参照してくださ](c-appendices/c-cgiparameters.md#reference_582E85C3886740C98FE88CA9DF7918E8)い。

## ライブ設定の表示 {#task_401A0EBDB5DB4D4CA933CBA7BECDC10F}

ステージされた任意のページで、設定のライブバージョンを確認できます。

<!-- 

t_viewing_live_settings.xml

 -->

このオプシ **[!UICONTROL View Live Settings]** ョンが有効（グレー表示）でない場合は、そのページのステージ設定とライブ設定が既に同期されています。

**ライブ設定を表示するには**

1. ステージ設定を含む任意のページで、をクリックし **[!UICONTROL View Live Settings]** て設定のライブバージョンを表示します。
1. 必要に応じて、次のいずれかの操作を行います。

   * をクリッ **[!UICONTROL View]** クして、ステージ設定に対して選択された現在のオプションを表示します。
   * をクリ **[!UICONTROL View Stage Settings]** ックして、設定を編集または削除できるステージ設定に戻ります。

## ステージ設定をライブにプッシュ {#task_44306783B4C0408AAA58B471DAF2D9A4}

設定は、任意のステージページビューまたは中央ページからライブにプッシュで **[!UICONTROL Manage Stage-Live Settings]** きます。

<!-- 

t_pushing_live_settings_live.xml

 -->

ページでこ **[!UICONTROL Push Live]** のオプションが有効（グレー表示されていない）場合は、ステージングされた設定があることを意味します。 または、設定に編集があり、保存すると設定がステージングされます。 このオプションをクリックすると、未保存の編集内容がステージ領域に保存されます。 保留中の編集がない場合、ページの設定は即座にライブにプッシュされます。

**ステージ設定をライブにプッシュするには**

1. 次のいずれかを実行します。

   * 「View」として「Staged」が選択されているページで、をクリックしま **[!UICONTROL Push Live]**&#x200B;す。
   * 製品メニューで、をクリックしま **[!UICONTROL Staging]**&#x200B;す。 ページで、 **[!UICONTROL Manage Stage-Live Settings]** 次のいずれかの操作を行います。

   * 設定ツリーを使用して、ライブにする設定のみを確認し、をクリックします **[!UICONTROL Push Selected Live]**。
   * クリック **[!UICONTROL Push All Live]**.

## 一元的な場所からのステージライブ設定の削除 {#task_B72BEA9269704B1399600A9CA273369B}

削除する設定が多数ある場合は、ページを使用して、1か所 **[!UICONTROL Manage Stage-Live Settings]** の一元的な場所から設定を削除できます。

<!-- 

t_deleting_staged_settings_from_a_central_location.xml

 -->

**警告**:をクリックすると、チ **[!UICONTROL Delete Selected]**&#x200B;ェックされたすべての設定が直ちに削除されます。選択した設定を本当に削除するかどうかを確認するダイアログボックスはありません。 また、ページに関連付けられた履歴機能はありません。 したがって、削除を元に戻すことはできません。

**ステージライブ設定を中央の場所から削除するには**

1. 製品メニューで、をクリックしま **[!UICONTROL Staging]**&#x200B;す。
1. ページ **[!UICONTROL Manage Stage-Live Settings]** で、設定ツリーを使用して、削除する設定のみを確認します。
1. クリック **[!UICONTROL Delete Selected]**.