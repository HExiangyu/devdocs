---
layout: default
group: install2
subgroup: Z_continue
title: Next&mdash;Choose how to install the Magento software
menu_title: Next&mdash;Choose how to install the Magento software
menu_node: parent
menu_order: 1
github_link: install-gde/continue.md
redirect_from: 
  - /guides/v1.0/install-gde/continue.html
  - /guides/v2.0/install-gde/install/pre-install.html
---

## 让我们开始吧!
本安装指南可以帮助您在没有安装过 Magento 的服务器上安装 Magento. (已经安装过? 请<a href="{{ site.gdeurl }}install-gde/basics/basics_magento-installed.html">点击这里</a>.)

<h2 id="install-overview-audience">选择如何安装 Magento 软件</h2>
想简单方便的安装Magento您需要使用 <a href="https://getcomposer.org/doc/00-intro.md" target="_blank">Composer</a>下载Magento2的代码?

如何开始，请参考下表.

<table>
	<!-- <col width="25%">
	<col width="65%">
	<col width="10%"> -->
	<tbody>
		<tr>
			<th>用户需要</th>
			<th>介绍</th>
			<th>高级安装步骤</th>
			<th>链接</th>
		</tr>
	<tr>
		<td><p>简单安装,不需要使用命令行, 有自己的服务器</p></td>
		<td><p>一些技术的专业知识，能对 Magento 服务器进行命令行访问.</p></td>
		<td><ol><li>下载一个压缩的文件，包含的 Magento 软件.</li>
			<li>Extracts it on the Magento server or asks a network administrator to do so.</li>
			<li>Installs the Magento software using the Setup Wizard or command line.</li></ol>
		</td>
		<td><p><a href="{{ site.gdeurl }}install-gde/prereq/zip_install.html">Easy installation (own server)</a></p></td>
	</tr>
	<tr>
		<td><p>Shared hosting, easy installation, no command line access</p></td>
		<td><p>Uses a hosting provider, has very little technical expertise, limited if any access to the Magento server.</p></td>
		<td><ol><li>Downloads a compressed file that contains the Magento software.</li>
			<li>Extracts it on the Magento server.</li>
			<li>Installs the Magento software using the Setup Wizard.</li></ol>
		</td>
		<td><p><a href="{{ site.gdeurl }}install-gde/install/hosted/hosted_start.html">Easy installation (shared hosting)</a></p></td>
	</tr>
	<tr>
		<td><p>Integrator, packager</p></td>
		<td><p>Wants full control over all components installed, has access to the Magento server, highly technical, might repackage Magento CE with other components.</p></td>
		<td><ol><li>Creates a Composer <em>project</em> that contains the list of components to use.</li>
			<li>Uses Composer to update package dependencies; uses <code>composer create-project</code> to get the Magento metapackage.</li>
			<li>Installs the Magento software using either a command line or the Setup Wizard.</li></ol>
		<td><p><a href="{{ site.gdeurl }}install-gde/prereq/integrator_install.html">Get the metapackage</a></p></td>
	</td>

	</tr>
	<tr>
		<td><p>Contributing developer</p></td>
		<td><p>Contributes to the Magento codebase, highly technical, has their own Magento development server, understands Composer and GitHub.</p></td>
		<td><ol><li>Clones the Magento 2 GitHub repository.</li>
			<li>Uses Composer to update package dependencies.</li>
			<li>Installs the Magento software using either a command line or the Setup Wizard.</li></ol>
		<td><p><a href="{{ site.gdeurl }}install-gde/prereq/dev_install.html">Clone the Magento repository</a></p></td>
	</td>
	</tr>
	
	
	</tbody>
</table>
