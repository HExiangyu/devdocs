# Magento中文开发文档

<<<<<<< HEAD
此项目为为Magento中文开发文档.也就是翻译Magento官方的开发手册.

如果您想参与到我们的翻译团队中，请联系QQ58573655
=======
Welcome! This site contains the latest Magento developer documentation for ongoing Magento 2.x releases.

To contribute, please fork the `develop` branch. 
>>>>>>> develop

### 请翻译的时候注意:

<<<<<<< HEAD
 *尽可能根据自己的理解翻译,能加上自己的见解最好，直译看着很难受不推荐。
 
 *尽可能统一名词翻译称谓，比如guide翻译为手册,extension翻译为扩展而不是插件.
 
#### 如何翻译?
 本项目MD相当于一个HTML的模板，直接翻译.md文件的内容就可以。



=======
You can build this site locally using Jekyll

*	Windows users _must_ build the site in a Vagrant container running on Virtual Box as discussed in more detail in the [Vagrant README](vagrant/README.md).

	We use symbolic links (symlinks) in the `guides/v2.1` directory to link to topics that haven't changed since the 2.0.x release. Because symlinks aren't supported by Windows, you _cannot_ use the Windows environment; you must use a Linux environment.

*	Mac and Linux users can build this site locally using Jekyll or you can use Vagrant. 

	Vagrant might be easier because the software runs in a container that isn't dependent on, and cannot conflict with, any other software installed on your computer.

## Build using Vagrant

To build the site locally using Vagrant you need only the files in the `vagrant/` directory.
For more information, see the [Vagrant README](vagrant/README.md).

## Requirements

Currently, building this site requires:

*	Ruby Version: >= 2.0.0

Use [bundler](http://bundler.io/) to get compatible versions of other dependencies.

## Build locally in Mac or Linux

To build this site locally:

```bash
# Install dependencies
$ bundle install

# Visit http://localhost:4000 in your favorite browser!
$ bin/jekyll serve --incremental
```
>>>>>>> develop

如果有任何问题，请联系下面:


*	<a href="https://twitter.com/MagentoDevDocs" class="twitter-follow-button" data-show-count="false">Follow @MagentoDevDocs</a>

*	<a href="mailto:DL-Magento-Doc-Feedback@magento.com">E-mail us</a>

*	<a href="http://devdocs.magento.com">Visit our documentation site</a>, built on GitHub using [Jekyll](http://jekyllrb.com/).

联系QQ群:9505614
