---
title: Renomear um repositório
intro: Você poderá renomear um repositório se for proprietário da organização ou tiver permissões de administrador no repositório.
redirect_from:
  - /articles/renaming-a-repository
  - /github/administering-a-repository/renaming-a-repository
  - /github/administering-a-repository/managing-repository-settings/renaming-a-repository
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Repositories
---

Quando você renomear um repositório, todas as informações existentes, com exceção das URLs do site do projeto, serão automaticamente redirecionadas para o novo nome, incluindo:

* Problemas
* Wikis
* Estrelas
* Seguidores

Para obter mais informações sobre sites de projeto, consulte "[Sobre {% data variables.product.prodname_pages %}](/pages/getting-started-with-github-pages/about-github-pages#types-of-github-pages-sites)".

Além do redirecionamento do tráfego da web, todas as operações `git clone`, `git fetch` ou `git push` direcionadas ao local antigo continuarão a funcionar como se tivessem sido criadas no novo local. No entanto, para reduzir a confusão, recomendamos que a atualização de quaisquer clones locais existentes apontem para a nova URL do repositório. Você pode fazer isso usando o `git remote` na linha de comando:

```shell
$ git remote set-url origin <em>new_url</em>
```

Para obter mais informações, consulte "[Gerenciar repositórios remotos](/github/getting-started-with-github/managing-remote-repositories)".

{% ifversion fpt or ghec %}

Se você planeja renomear um repositório que tenha um site do {% data variables.product.prodname_pages %} , recomendamos usar um domínio personalizado para o seu site. Isso garante que a URL do site não seja impactada pela renomeação do repositório. Para obter mais informações, consulte "[Sobre um domínio personalizado e o site {% data variables.product.prodname_pages %}](/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages)".

{% endif %}

{% note %}

**Note:** {% data variables.product.prodname_dotcom %} will not redirect calls to an action hosted by a renamed repository. Any workflow that uses that action will fail with the error `repository not found`. Instead, create a new repository and action with the new name and archive the old repository. Para obter mais informações, consulte "[Arquivando repositórios](/repositories/archiving-a-github-repository/archiving-repositories)".

{% endnote %}

{% warning %}

**Aviso**: Se você criar um novo repositório em sua conta no futuro, não reutilize o nome original do repositório renomeado. Se o fizer, o redirecionamento para o repositório renomeado quebrará.

{% endwarning %}

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
3. No cabeçalho **Repository Name** (Nome do repositório), insira o novo nome do repositório. ![Renomeação do repositório](/assets/images/help/repository/repository-name-change.png)
4. Clique em **Rename** (Renomear). Pronto!