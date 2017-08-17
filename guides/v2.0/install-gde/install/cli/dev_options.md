---
layout: default
group: install_cli 
subgroup: 99_contrib
title: 协助开发人员&mdash;更新, 重装Magento
menu_title: 协助开发人员&mdash;更新, 重装Magento
menu_order: 1
menu_node: parent
version: 2.0
github_link: install-gde/install/cli/dev_options.md
redirect_from: 
  - guides/v2.0/install-gde/install/dev_updater.html
  - guides/v2.1/install-gde/install/dev_updater.html
---

以下内容只对使用`git clone`从Github代码库安装的用户适用. 这通常意味着你贡献过代码到Magento CE 代码库。

<<<<<<< HEAD
*	<a href="{{ site.gdeurl }}install-gde/install/cli/dev_update-magento.html">更新Magento</a>, 使用 `git pull origin` 和 `composer update`
*	<a href="{{ site.gdeurl }}install-gde/install/cli/dev_add-update.html">添加, 删除,或者更新组件</a>, 修改 `composer.json` 并运行 `composer update`
*	<a href="{{ site.gdeurl }}install-gde/install/cli/dev_reinstall.html">重新安装Magento</a>, 在 `composer.json`中修改版本号,并运行 `composer update`，重新安装Magento2.

<div class="bs-callout bs-callout-info" id="info">
	<span class="glyphicon-class">
		<p>如果你不是贡献开发者,您执行升级和升级讨论在<a href="{{ site.gdeurl }}comp-mgr/bk-compman-upgrade-guide.html">更新Magento和组件</a>.</p> </span>
=======
<div class="bs-callout bs-callout-warning">
    <p>If you clone the Magento 2 GitHub repository, you <em>cannot</em> use the Magento software in a production environment. You cannot have a live store that accepts orders and so on.</p>
</div>

*	To <a href="{{page.baseurl}}install-gde/install/cli/dev_update-magento.html">update the Magento software</a>, use `git pull origin` and `composer update`, then update the Magento database
*	To <a href="{{page.baseurl}}install-gde/install/cli/dev_downgrade.html">change versions</a> from `develop` to a release version like `2.0.4`, you must uninstall the Magento software and install the released version.
*	To <a href="{{page.baseurl}}install-gde/install/cli/dev_add-update.html">add, remove, or update components</a>, modify `composer.json` and run `composer update` and update the Magento database
*	To <a href="{{page.baseurl}}install-gde/install/cli/dev_reinstall.html">reinstall the Magento software</a>, modify the product version in `composer.json`, run `composer update`, then reinstall the Magento software

<div class="bs-callout bs-callout-info" id="info">
	<span class="glyphicon-class">
		<p>If you are not a contributing developer, you perform upgrades and upgrades as discussed in <a href="{{page.baseurl}}comp-mgr/bk-compman-upgrade-guide.html">Updating the Magento application and components</a>.</p> </span>
>>>>>>> develop
</div>

<!-- ABBREVIATIONS -->

<<<<<<< HEAD
*[贡献开发者]: 向Mageno2代码库贡献过代码的开发人员
=======
*[contributing developer]: A developer who contributes code to the Magento 2 CE codebase
>>>>>>> develop
