# Qiniu Resource (Cloud) Storage SDK for Ruby

## 关于

此 Ruby SDK 基于 [七牛云存储官方API](http://developer.qiniu.com/docs/v6/index.html) 构建。使用此 SDK 构建您的网络应用程序，能让您以非常便捷地方式将数据安全地存储到七牛云存储上。无论您的网络应用是一个网站程序，还是包括从云端（服务端程序）到终端（手持设备应用）的架构的服务或应用，通过七牛云存储及其 SDK，都能让您应用程序的终端用户高速上传和下载，同时也让您的服务端更加轻盈。

支持的 Ruby 版本：

* Ruby 2.1.x
* Ruby 2.2.x
* Ruby 2.3.x
* JRuby 9.x

如果您的应用程序需要在 Ruby 1.9、2.0 或 JRuby 1.7 上运行，请使用此 Ruby SDK 的 6.6.0 版本。

## 状态

[![Build Status](https://api.travis-ci.org/qiniu/ruby-sdk.png?branch=master)](https://travis-ci.org/qiniu/ruby-sdk)
[![Gem Version](https://badge.fury.io/rb/qiniu.png)](http://badge.fury.io/rb/qiniu)
[![Dependency Status](https://gemnasium.com/qiniu/ruby-sdk.png)](https://gemnasium.com/qiniu/ruby-sdk)
[![Code Climate](https://codeclimate.com/github/qiniu/ruby-sdk.png)](https://codeclimate.com/github/qiniu/ruby-sdk)

## 安装

在您 Ruby 应用程序的 `Gemfile` 文件中，添加如下一行代码：

    gem 'qiniu', '=> 6.4.1', '<= 6.6.0'

然后，在应用程序所在的目录下，可以运行 `bundle` 安装依赖包：

    $ bundle

或者，可以使用 Ruby 的包管理器 `gem` 进行安装：

    $ gem install qiniu

## Rails 4 项目安装

在 Rails 4 项目的 `Gemfile` 里添加 `qiniu` 后执行 `bundle` 命令可能会失败，这是因为 Rails 4 项目默认会使用 `mime-types` 3.x 版本。需要使用以下命令将 `mime-types` 降级为满足 Qiniu Ruby SDK 的 2.6.x 版本。

    bundle update mime-types

由于 `mime-types` 3.0 要求的最低 Ruby 版本是 2.0，而 Qiniu Ruby SDK 支持 Ruby 1.9，因此我们不能通过简单修改对 `mime-types` 的版本依赖来解决此问题。

## 使用

参考文档：[七牛云存储 Ruby SDK 使用指南](http://developer.qiniu.com/docs/v6/sdk/ruby-sdk.html)

## 贡献代码

1. Fork
2. 创建您的特性分支 (`git checkout -b my-new-feature`)
3. 提交您的改动 (`git commit -am 'Added some feature'`)
4. 将您的修改记录提交到远程 `git` 仓库 (`git push origin my-new-feature`)
5. 然后到 github 网站的该 `git` 远程仓库的 `my-new-feature` 分支下发起 Pull Request

## 许可证

Copyright (c) 2012-2014 qiniu.com

基于 MIT 协议发布:

* [www.opensource.org/licenses/MIT](http://www.opensource.org/licenses/MIT)

