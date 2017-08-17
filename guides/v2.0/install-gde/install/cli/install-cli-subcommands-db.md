---
layout: default
group: install_cli 
subgroup: 05_Command-line installation
title: 创建 Magento2 数据库架构
menu_title: 创建 Magento2 数据库架构
menu_node: 
menu_order: 15
version: 2.0
github_link: install-gde/install/cli/install-cli-subcommands-db.md
redirect_from: 
  -  /guides/v1.0/install-gde/install/install-cli-subcommands-db.html
  -  /guides/v2.0/install-gde/install/install-cli-subcommands-db.html
---

<<<<<<< HEAD
  
<h4>内容索引</h4>

请参见以下各节之一:

*	<a href="#instgde-install-cli-first">第一步</a>
*	<a href="#instgde-cli-subcommands-store-prereq">系统必备组件</a>
*	<a href="#instgde-cli-dbconfig">配置数据库和添加数据</a>


<h2 id="instgde-cli-before">第一步</h2>
{% include install/first-steps-cli.html %}
关于命令行的参数,请看<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-subcommands.html#instgde-cli-subcommands-common">Magento2命令行参数</a>.

<h2 id="instgde-cli-subcommands-db-prereq">系统必备组件</h2>
运行命令之前您必须<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-subcommands-deployment.html">创建或更新的部署配置</a>.
=======
<h2 id="instgde-cli-before">First steps</h2>
{% include install/first-steps-cli.html %}
In addition to the command arguments discussed here, see <a href="{{page.baseurl}}install-gde/install/cli/install-cli-subcommands.html#instgde-cli-subcommands-common">Common arguments</a>.

<h2 id="instgde-cli-subcommands-db-prereq">Prerequisites</h2>
Before you run this command, you must <a href="{{page.baseurl}}install-gde/install/cli/install-cli-subcommands-deployment.html">Create or update the deployment configuration</a>.
>>>>>>> develop

<h2 id="instgde-cli-dbconfig">配置数据库和添加数据</h2>
使用命令:

	magento setup:db-schema:upgrade
	magento setup:db-data:upgrade

如果需要查看数据库状态，请输入

	magento setup:db:status

<<<<<<< HEAD
#### 相关主题

*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-install.html">使用命令行安装Magento2</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-subcommands-enable.html">激活或者禁用Magento2模块</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-uninstall-mods.html">卸载模块</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-subcommands-deployment.html">创建部署配置</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-subcommands-maint.html">激活或者禁用Magento2维护模式</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-subcommands-db.html">创建 Magento 数据库架构</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-subcommands-store.html">配置存储</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-backup.html">备份文件, media和数据库</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-theme-uninstall.html">卸载Magento2主题</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-uninstall-langpk.html">卸载Magento2语言包</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-uninstall.html#instgde-install-uninstall">卸载Magento2</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-uninstall.html#instgde-install-magento-update">更新Magento2</a>
*	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-uninstall.html#instgde-install-magento-reinstall">重装Magento2</a>
=======
#### Related topics

*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-install.html">Installing the Magento software using the command line</a>
*	[Remove sample data modules or update sample data]({{ page.baseurl }}install-gde/install/cli/install-cli-sample-data-other.html)
*	[Enable or disable modules]({{ page.baseurl }}install-gde/install/cli/install-cli-subcommands-enable.html)
*	[Display or change the Admin URI]({{ page.baseurl }}install-gde/install/cli/install-cli-adminurl.html)
*	[Uninstall modules]({{ page.baseurl }}install-gde/install/cli/install-cli-uninstall-mods.html)
*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-subcommands-deployment.html">Create or update the deployment configuration</a>
*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-subcommands-maint.html">Enable or disable maintenance mode</a>
*	[Update the Magento database schema and data]({{ page.baseurl }}install-gde/install/cli/install-cli-subcommands-db-upgr.html)
*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-subcommands-store.html">Configure the store</a>
*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-subcommands-admin.html">Create or unlock a Magento administrator</a>
*	[Back up and roll back the file system, media, and database]({{ page.baseurl }}install-gde/install/cli/install-cli-backup.html)
*	[Uninstall themes]({{ page.baseurl }}install-gde/install/cli/install-cli-theme-uninstall.html)
*	[Uninstall language packages]({{ page.baseurl }}install-gde/install/cli/install-cli-uninstall-langpk.html)
*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-uninstall.html#instgde-install-uninstall">Uninstall the Magento software</a>
*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-uninstall.html#instgde-install-magento-update">Update the Magento software</a>
*	<a href="{{page.baseurl}}install-gde/install/cli/install-cli-uninstall.html#instgde-install-magento-reinstall">Reinstall the Magento software</a>
>>>>>>> develop
