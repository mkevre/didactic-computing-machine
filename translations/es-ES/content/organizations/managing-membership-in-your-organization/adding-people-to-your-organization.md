---
title: Agregar personas a tu organización
intro: 'Puedes hacer que cualquier persona se convierta en miembro de tu organización usando el nombre de usuario de {% data variables.product.product_name %} o la dirección de correo electrónico.'
redirect_from:
  - /articles/adding-people-to-your-organization
  - /github/setting-up-and-managing-organizations-and-teams/adding-people-to-your-organization
versions:
  ghes: '*'
  ghae: '*'
permissions: Organization owners can add people to an organization.
shortTitle: Agregar a las personas a una organización
---

{% ifversion not ghae %}
Si tu organización[requiere que los miembros usen autenticación de dos factores](/articles/requiring-two-factor-authentication-in-your-organization), los usuarios deben [habilitar la autenticación de dos factores](/articles/securing-your-account-with-two-factor-authentication-2fa) antes de que puedas agregarlos a la organización.
{% endif %}

{% data reusables.profile.access_org %}
{% data reusables.user-settings.access_org %}
{% data reusables.organizations.people %}
{% data reusables.organizations.invite_member_from_people_tab %}
{% data reusables.organizations.invite_to_org %}
{% data reusables.organizations.choose-to-restore-privileges %}
{% data reusables.organizations.choose-user-role %}
{% data reusables.organizations.choose-user-license %}
{% data reusables.organizations.add-user-to-teams %}
{% data reusables.organizations.send-invitation %}

## Leer más
- "[Agregar miembros de la organización a un equipo](/articles/adding-organization-members-to-a-team)"
