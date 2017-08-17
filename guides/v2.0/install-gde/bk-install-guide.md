---
layout: default
group: install2
subgroup: Getting Started
<<<<<<< HEAD
title: 安装概述
menu_title: 安装概述
menu_node: 
=======
title: How to get the Magento software
landing-page: Installation Guide
menu_title: How to get the Magento software
menu_node:
>>>>>>> develop
menu_order: 1
version: 2.0
github_link: install-gde/bk-install-guide.md
redirect_from:
  - /guides/v2.0/install-gde/continue.html
  - /guides/v2.1/install-gde/continue.html
  - /guides/v1.0/install-gde/bk-install-guide.html
  - /guides/v2.0/install-gde/install/install-merchbeta.html
---

<<<<<<< HEAD
<h2>Magento软件安装</h2>
你好,欢迎你选择全球240000家商家共同的使用和信任的Magento.我们收集了一些信息，帮助您入门 Magento 与 Magento 安装。
=======
## Magento software installation

Hi, we're glad you're among the 240,000 merchants worldwide who put their trust in our eCommerce software. We've gathered some information to help you get started with Magento and with your Magento installation.
>>>>>>> develop

我们这里有一些资源以帮助您开始使用未来的电子商务平台&mdash;Magento 2.

It’s what we do.

<<<<<<< HEAD
<h2 id="install-how-install">第一步,选择如何安装您的Magento</h2>
<a href="{{ site.gdeurl }}install-gde/continue.html">选择如何安装您的Magento</a>.

<h2 id="install-verify-prereq">第二步,Magento运行需要的一些必备组件</h2>
使用下表来验证您具有正确的Magento需要的系统必备组件。如果您使用共享的托管服务提供商，您可以跳过此步骤。
=======
## How to get the Magento software {#install-get-software}

Consult the following table for how to get started installing Magento Community Edition (CE) or Magento Enterprise Edition (EE).
>>>>>>> develop

<table>
	<tbody>
		<tr>
<<<<<<< HEAD
			<th>前提条件</th>
			<th>如何检查</th>
			<th>更多信息</th>
		</tr>
	<tr>
		<td><p>Apache 2.2 or 2.4</p></td>
		<td><p>Ubuntu: <code>apache2 -v</code></p>
		<p>CentOS: <code>httpd -v</code></p></td>
		<td><p><a href="{{ site.gdeurl }}install-gde/prereq/apache.html">Apache</a></p>
			<p>(不要忘了<a href="{{ site.gdeurl }}install-gde/prereq/apache.html#apache-help-rewrite">激活rewrites和 <code>.htaccess</code></a>!)</p></td>
	</tr>
	<tr>
		<td><p>PHP 5.6.x or 5.5.x PHP7+ (PHP 5.4已不支持)</p>
			<p>如何<a href="{{ site.gdeurl }}install-gde/trouble/tshoot_install-issues.html#known-devrc-php">查看自己的php版本</a></p></td>
		<td><p><code>php -v</code></p></td>
		<td><a href="{{ site.gdeurl }}install-gde/prereq/php-ubuntu.html">PHP Ubuntu</a><br><a href="{{ site.gdeurl }}install-gde/prereq/php-centos.html">PHP CentOS</a></td>
=======
			<th>User needs</th>
			<th>Description</th>
			<th>High-level installation and upgrade steps</th>
			<th>Get started link</th>
		</tr>
	<tr>
		<td><p>Easy installation, command line, have your own server</p></td>
		<td><p>Some technical expertise, command line access to the Magento server.</p>
			<p>Enables you to install the Magento software and extensions using either the <a href="{{ page.baseurl }}install-gde/install/web/install-web.html">Web Setup Wizard</a> or the <a href="{{ page.baseurl }}install-gde/install/cli/install-cli.html">command line</a>.</p>
		<p>You <em>cannot</em> use the Web Setup Wizard to upgrade the Magento software and extensions. You must upgrade using <a href="{{page.baseurl}}/install-gde/install/cli/dev_reinstall.html">Composer</a> and the <a href="{{page.baseurl}}install-gde/install/cli/install-cli.html">command line</a>.</p></td>
		<td><ol><li>Downloads a compressed file that contains the Magento software.</li>
			<li>Extracts it on the Magento server or asks a network administrator to do so.</li>
			<li>Installs the Magento software using the Web Setup Wizard or command line.</li>
			<li>Upgrades the Magento application and extensions using Composer and the command line.</li></ol>
		</td>
		<td><p><a href="{{page.baseurl}}install-gde/prereq/zip_install.html">Easy installation (own server)</a></p></td>
	</tr>
	<tr>
		<td><p>Integrator, packager</p></td>
		<td><p>Wants full control over all components installed, has access to the Magento server, highly technical, might repackage Magento CE with other components.</p>
		<p>Enables you to install the Magento software and extensions using either the <a href="{{ page.baseurl }}install-gde/install/web/install-web.html">Web Setup Wizard</a> or the <a href="{{ page.baseurl }}install-gde/install/cli/install-cli.html">command line</a>.</p>
		<p>You can also upgrade the Magento application and extensions using the <a href="{{ page.baseurl }}comp-mgr/bk-compman-upgrade-guide.html">Web Setup Wizard</a> or <a href="{{ page.baseurl }}comp-mgr/cli/cli-upgrade.html">command line</a>.</p></td>
		<td><ol><li>Creates a Composer <em>project</em> that contains the list of components to use.</li>
			<li>Uses Composer to update package dependencies; uses <code>composer create-project</code> to get the Magento metapackage.</li>
			<li>Installs the Magento software using either a command line or the Setup Wizard.</li>
		<li>Upgrades the Magento application and extensions using the Web Setup Wizard or command line.</li></ol>
		<td><p><a href="{{page.baseurl}}install-gde/prereq/integrator_install.html">Get the metapackage</a></p></td>
	</td>

>>>>>>> develop
	</tr>
	<tr>
		<td><p>Contributing developer</p></td>
		<td><p>Contributes to the Magento codebase, files bugs, and customizes the Magento software. Highly technical, has their own Magento development server, understands Composer and GitHub.</p>
			<p>Enables you to install the Magento software and extensions using either the <a href="{{ page.baseurl }}install-gde/install/web/install-web.html">Web Setup Wizard</a> or the <a href="{{ page.baseurl }}install-gde/install/cli/install-cli.html">command line</a>.</p>
			<p>You <em>cannot</em> use Magento in a production environment.</p>
      <p>You <em>cannot</em> use the Web Setup Wizard to upgrade the Magento software and extensions. You must upgrade using <a href="{{page.baseurl}}/install-gde/install/cli/dev_options.html">Composer and git commands</a>.</p></td>
		<td><ol><li>Clones the Magento 2 GitHub repository.</li>
			<li>Uses Composer to update package dependencies.</li>
			<li>Installs the Magento software using either a command line or the Setup Wizard.</li>
			<li>Upgrades the Magento software using Composer and GitHub commands.</li>
			<li>Customizes code under the <code>app/code</code> directory.</li></ol></td>
		<td><p><a href="{{page.baseurl}}install-gde/prereq/dev_install.html">Clone the Magento repository</a></p></td>
	</tr>
<<<<<<< HEAD
</tbody>
</table>

<h2>第三步，安装 Magento</h2>
*	简单安装: <a href="{{ site.gdeurl }}install-gde/install/web/install-web.html">使用Magento向导进行安装</a>

	<a href="{{ site.gdeurl }}install-gde/install/web/install-web-sample-data.html">安装演示数据(基于Magento向导)</a>
*	高级安装: <a href="{{ site.gdeurl }}install-gde/install/cli/install-cli.html">使用命令行安装Magento</a>

	<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli-sample-data.html">安装演示数据(基于命令行)</a>

<h2>安装后</h2>
*	<a href="{{ site.gdeurl }}install-gde/install/verify.html">验证安装</a>
*	<a href="{{ site.gdeurl }}install-gde/trouble/tshoot.html">疑难解答</a>
*	<a href="{{ site.gdeurl }}install-gde/install/sample-data-after-magento.html">安装Magento后安装演示数据</a>
*	<a href="{{ site.gdeurl }}install-gde/install/post-install-config.html">配置</a>

<h2>有用的信息</h2>
在您的安装过程中, 可以使用我们的<a href="{{ site.gdeurl }}install-gde/install-quick-ref.html">快速安装参考 (教程)</a>或者<a href="{{ site.gdeurl }}install-gde/install-roadmap_part1.html">安装指南 (引用)</a>. 这些教程都是很简单的，本教程将指导你安装一个带演示数据的Magento。
=======


	</tbody>
</table>

## Useful information

At any time during your installation, take advantage of our [installation quick reference (tutorial)] or [installation roadmap (reference)]. They're really easy to use; the tutorial walks you through a sample installation. The roadmap provides links to common tasks throughout the guide.
>>>>>>> develop

使用左侧导航，可以安装其他部分。

<<<<<<< HEAD
<h2>必须的服务器权限</h2>
UNIX系统需要 `root` 权限来安装配置PHP,Composer,Grunt等，到你的服务器.如果需要安装,请确保您有 `root`权限.

您不能使用ROOT权限作为Magento的文件权限,因为Root权限可能造成webserver不能访问Magento。

您还需要 `root`权限来创建 <a href="{{ site.gdeurl }}install-gde/prereq/apache-user.html">Magento文件权限所有者(owner)</a>并添加所有者( owner)到您的webserver用户组. 要从命令行(Cli)运行任何命令，并设置 Magento cron，您将使用 Magento 文件系统所有者.
=======
## Required server permissions

UNIX systems require `root` privileges to install and configure software like a web server, PHP, and so on. If you need to install this software, make sure you have `root` access.

You should *not* install the Magento software in the web server docroot as the `root` user because the web server might not be able to interact with those files.

You'll also need `root` privileges to create the [Magento file system owner] and add that owner to the web server's group. You'll use the {% glossarytooltip 5e7de323-626b-4d1b-a7e5-c8d13a92c5d3 %}Magento file system owner{% endglossarytooltip %} to run any commands from the command line and to set up the Magento cron job, which schedules tasks for you.

<!-- LINK DEFINITIONS -->

[installation quick reference (tutorial)]: {{page.baseurl}}install-gde/install-quick-ref.html
[installation roadmap (reference)]: {{page.baseurl}}install-gde/install-roadmap_part1.html
[Magento file system owner]: {{page.baseurl}}install-gde/prereq/file-sys-perms-over.html
>>>>>>> develop
