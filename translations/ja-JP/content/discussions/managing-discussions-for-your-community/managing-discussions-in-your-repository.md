---
title: リポジトリ内のディスカッションを管理する
intro: リポジトリ内のディスカッションを分類、スポットライト、転送、または削除できます。
permissions: Repository administrators and people with write or greater access to a repository can manage discussions in the repository.
versions:
  fpt: '*'
  ghec: '*'
shortTitle: Manage discussions
---


## ディスカッションの管理について

{% data reusables.discussions.about-discussions %}ディスカッションに関する詳しい情報については「[ディスカッションについて](/discussions/collaborating-with-your-community-using-discussions/about-discussions)」を参照してください。

Organization のオーナーは、Organization が所有するリポジトリのディスカッションを作成するために必要な権限を選択できます。 詳しい情報については、「[Organization 内のリポジトリのディスカッションの作成を管理する](/organizations/managing-organization-settings/managing-discussion-creation-for-repositories-in-your-organization)」を参照してください。

ディスカッションのメンテナとして、コミュニティリソースを作成して、プロジェクト全体の目標に沿ったディスカッションを促し、コラボレータのための親しみやすいオープンフォーラムを維持できます。 コラボレータが従う行動規範またはコントリビューションガイドラインを作成することは、協力的で生産的なフォーラムを促進するのに役立ちます。 コミュニティリソースの作成について詳しくは、「[プロジェクトに行動規範を追加する](/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project)」および 「[リポジトリコントリビューター向けのガイドラインを設定する](/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors)」を参照してください。

When a discussion yields an idea or bug that is ready to be worked on, you can create a new issue from a discussion. 詳しい情報については、「[Issue を作成する](/issues/tracking-your-work-with-issues/creating-an-issue#creating-an-issue-from-a-discussion)」を参照してください。

健全なディスカッションの促進について詳しくは、「[コメントと会話のモデレーション](/communities/moderating-comments-and-conversations)」を参照してください。

{% data reusables.discussions.you-can-label-discussions %}

## 必要な環境

To manage discussions in a repository, {% data variables.product.prodname_discussions %} must be enabled for the repository. For more information, see "[Enabling or disabling {% data variables.product.prodname_discussions %} for a repository](/github/administering-a-repository/enabling-or-disabling-github-discussions-for-a-repository)."

## ディスカッションのカテゴリを変更する

ディスカッションを分類して、コミュニティメンバーが関連するディスカッションを見つけやすくすることができます。 詳しい情報については、「[リポジトリ内のディスカッションのカテゴリを管理する](/discussions/managing-discussions-for-your-community/managing-categories-for-discussions-in-your-repository)」を参照してください。

ディスカッションを別のカテゴリに移動することもできます。

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.discussions.discussions-tab %}
{% data reusables.discussions.click-discussion-in-list %}
1. In the right sidebar, to the right of "Category", click {% octicon "gear" aria-label="The gear icon" %}. !["Category" with gear icon](/assets/images/help/discussions/category-in-sidebar.png)
1. Click a category. !["Change category" drop-down menu](/assets/images/help/discussions/change-category-drop-down.png)

## ディスカッションをピン留めする

リポジトリのディスカッションのリストに、最大 4 つの重要なディスカッションをピン留めできます。

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.discussions.discussions-tab %}
{% data reusables.discussions.click-discussion-in-list %}
1. 右のサイドバーで、{% octicon "pin" aria-label="The pin icon" %} [**Pin discussion**] をクリックします。 ![ディスカッションの右のサイドバーにある [Pin discussion]](/assets/images/help/discussions/click-pin-discussion.png)
1. 必要に応じて、ピン留めされたディスカッションの外観をカスタマイズします。 ![ピン留めされたディスカッションのカスタマイズオプション](/assets/images/help/discussions/customize-pinned-discussion.png)
1. [**Pin discussion**] をクリックします。 ![ピン留めされたディスカッションのカスタマイズオプションの下にある [Pin discussion] ボタン](/assets/images/help/discussions/click-pin-discussion-button.png)

## ピン留めされたディスカッションを編集する

ピン留めされたディスカッションを編集しても、ディスカッションのカテゴリは変更されません。 詳しい情報については、「[リポジトリ内のディスカッションのカテゴリを管理する](/discussions/managing-discussions-for-your-community/managing-categories-for-discussions-in-your-repository)」を参照してください。

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.discussions.discussions-tab %}
{% data reusables.discussions.click-discussion-in-list %}
1. 右のサイドバーで、{% octicon "pencil" aria-label="The pencil icon" %} [**Edit pinned discussion**] をクリックします。 !["Edit pinned discussion" in right sidebar for discussion](/assets/images/help/discussions/click-edit-pinned-discussion.png)
1. ピン留めされたディスカッションの外観をカスタマイズします。 ![ピン留めされたディスカッションのカスタマイズオプション](/assets/images/help/discussions/customize-pinned-discussion.png)
1. [**Pin discussion**] をクリックします。 ![ピン留めされたディスカッションのカスタマイズオプションの下にある [Pin discussion] ボタン](/assets/images/help/discussions/click-pin-discussion-button.png)

## ディスカッションをピン留め解除する

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.discussions.discussions-tab %}
{% data reusables.discussions.click-discussion-in-list %}
1. 右のサイドバーで、{% octicon "pin" aria-label="The pin icon" %} [**Unpin discussion**] をクリックします。 ![ディスカッションの右のサイドバーにある [Unpin discussion]](/assets/images/help/discussions/click-unpin-discussion.png)
1. 警告を読み、[**Unpin discussion**] をクリックします。 ![モーダルの警告の下にある [Unpin discussion] ボタン](/assets/images/help/discussions/click-unpin-discussion-button.png)

## ディスカッションを移譲する

ディスカッションを移譲するには、ディスカッションを移譲するリポジトリにディスカッションを作成する権限が必要です。 You can only transfer discussions between repositories owned by the same user or organization account. You can't transfer a discussion from a private repository to a public repository.

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.discussions.discussions-tab %}
{% data reusables.discussions.click-discussion-in-list %}
1. 右のサイドバーで、{% octicon "arrow-right" aria-label="The right arrow icon" %} [**Transfer discussion**] をクリックします。 ![ディスカッションの右のサイドバーにある [Transfer discussion]](/assets/images/help/discussions/click-transfer-discussion.png)
1. [**Choose a repository**] ドロップダウンを選択し、ディスカッションの移譲先のリポジトリをクリックします。 ![[Choose a repository] ドロップダウン、[Find a repository] 検索フィールド、およびリスト内のリポジトリ](/assets/images/help/discussions/use-choose-a-repository-drop-down.png)
1. [**Transfer discussion**] をクリックします。 ![[Transfer discussion] ボタン](/assets/images/help/discussions/click-transfer-discussion-button.png)

## ディスカッションを削除する

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.discussions.discussions-tab %}
{% data reusables.discussions.click-discussion-in-list %}
1. 右のサイドバーで、{% octicon "trash" aria-label="The trash arrow icon" %} [**Delete discussion**] をクリックします。 ![ディスカッションの右のサイドバーにある [Delete discussion]](/assets/images/help/discussions/click-delete-discussion.png)
1. 警告を読み、[**Delete this discussion**] をクリックします。 ![モーダルの警告の下にある [Delete this discussion] ボタン](/assets/images/help/discussions/click-delete-this-discussion-button.png)

## ラベルに基づいて Issue を変換する

同じラベルのすべての Issue をまとめてディスカッションに変換できます。 このラベルの今後の Issue も、設定したディスカッションとカテゴリに自動的に変換されます。

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-issues %}
{% data reusables.project-management.labels %}
1. Issue に変換するラベルの横にある [**Convert issues**] をクリックします。
1. [**Choose a category**] ドロップダウンメニューを選択し、ディスカッションのカテゴリをクリックします。
1. [**I understand, convert this issue to a discussion**] をクリックします。
