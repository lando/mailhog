---
description: All Other documentation versions
title: Docuverse
contributors: false
lastUpdated: false
editLink: false
next: false
prev: false
---
# Docuverse

<br />
<br />

<div
  v-for="link in links"
  :key="link.text"
  class="version-link"
>
  <VPLVersionLink
    :version="link.text"
    :prerelease="link.prerelease"
    :stable="link.stable"
    :edge="link.edge"
  />
</div>

<br />

<div>
  <VPLVersionLink :dev="true" :version="aliases.dev" />
</div>

<script setup>
import {useTags} from '@lando/vitepress-theme-default-plus';
import {VPLCollectionPage, VPLCollectionPageSection, VPLCollectionPageTitle, VPLVersionLink} from '@lando/vitepress-theme-default-plus';

const {aliases, aliasLinks, links} = useTags();
</script>
