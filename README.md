# Acrolinx Classic Edition SDKs

The following instructions and sample code will help you integrate [Acrolinx](http://www.acrolinx.com/)
in Java, .NET, or C++ applications.
The SDKs take care of most of the functionality for you, so you can develop integrations quickly.

## New Acrolinx Platform API

Acrolinx develops a new [Platform API](https://github.com/acrolinx/platform-api).
If you start a new project, you might want to use the new API instead of the classic.

## Automated or Authoring Integration

Acrolinx Integrations serve two main use cases.

### 1. Interactive, Authoring Integration

You can integrate Acrolinx in an authoring environment to give writers feedback while they edit content.
For example, you might want to build an Acrolinx Integration for a desktop XML editor.

### 2. Embedded Integration

You can integrate Acrolinx in a server application to enable (automated) batch checking over a set of documents.
For example, you might integrate Acrolinx in your CMS to check content as an automated workflow step.

## What Is the Difference Between Sidebar and Classic Edition?

Acrolinx Integrations now come in [two different editions](https://support.acrolinx.com/hc/en-us/articles/208549775).

The classic edition is the predecessor to the Sidebar. With a classic edition integration,
writers can check and edit their content with the help of a shortcut menu that appears when they click colored issues.

The Sidebar is the newest edition in the Acrolinx Integration family.
We've invested in this technology to provide a cross-platform SDK with a modern user experience.
We've also simplified the API for integrators so you can build an Acrolinx Integration by implementing a few methods
and writing just a couple of lines of code.

If you'd like to build an authoring integration, we strongly recommend using the Acrolinx Sidebar.

See: [Recommendations](#recommendations)

## Prerequisites

Please contact Acrolinx SDK support (sdk-support@acrolinx.com) for consulting and getting your integration certified.

## Before You Start

Check out our [Guidance for the Development of Acrolinx Integrations](https://github.com/acrolinx/acrolinx-coding-guidance).
Not all points might make sense for your current project, or your company might have its own guidelines for writing code.
This document is designed to help you avoid common pitfalls when you develop an Acrolinx Integration.

## Recommendations

### Develop an Authoring Integration

#### JavaScript

If you're developing a web-based Acrolinx Integration, have a look at [Acrolinx Sidebar Demo](https://github.com/acrolinx/acrolinx-sidebar-demo).

#### .NET

See: [Acrolinx Sidebar .NET](https://github.com/acrolinx/acrolinx-sidebar-demo-dotnet)

#### You Haven't Found a Sidebar SDK in Your Favorite Coding Language?

To run the [Sidebar](https://github.com/acrolinx/acrolinx-sidebar-demo) using your favorite coding language,
you just need to load the Sidebar in a web browser control and interact with the JavaScript inside.

Before you start building a new Acrolinx SDK on your own, contact Acrolinx SDK support (sdk-support@acrolinx.com).
Chances are we're working on a Sidebar SDK in the language you want to use...

### Develop an Embedded Integration

The standalone [Content Analyzer](https://support.acrolinx.com/hc/en-us/articles/211749485)
might already sufficiently cover your use case for analyzing your content from an entire folder structure or website.

To run Acrolinx repeatedly as an automated task, you can use the [Command-Line Checker](https://support.acrolinx.com/hc/en-us/articles/203943742).
The [Acrolinx Scorecard Analyzer project](https://github.com/acrolinx/acrolinx-scale#how-to-use-the-acrolinx-command-line-checker-to-perform-a-check)
provides a script-based example of using the Command-Line Checker.

You can automatically run the Command-Line Checker, for example,
in a post-commit-hook of your source code repository like GIT, started by a continuous integration system like Jenkins,
or run it by a task scheduler like cron or the Windows Task Scheduler.

The Acrolinx Java SDK is another option for using Acrolinx in an embedded integration.

## Acrolinx Java SDK

### [Getting Started with Acrolinx Java SDK Snippets](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/5750a55d31d0d5fe267e75c768660f5f7d42c606/java-sdk/html/snippets.html)

### [JavaDoc of Acrolinx Java SDK](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/5750a55d31d0d5fe267e75c768660f5f7d42c606/java-sdk/html/apidocs/index.html)

### The Acrolinx Java SDK in Action - Starting the Demo Integration

To see the Acrolinx Java SDK in action, execute the file `demo-projects/startable-swing-gui/java-sdk-gui-swing-sample.bat`.

#### To See the SWT Version of the Acrolinx Java SDK

1. Goto: `demo-projects/startable-swt-gui/`
2. Download correct SWT version depending on your environment: java VM + os from [eclipse.org/swt](https://www.eclipse.org/swt/).
3. Extract the downloaded archive and copy the `swt.jar` to `demo-projects/startable-swt-gui/`
4. Start `java-sdk-gui-swt-sample.bat`

### First Steps with the Acrolinx Java SDK

1. Create a new java project
2. Copy the Acrolinx Java SDK jar into your project
3. Import this jar into the classpath of your new project
4. Take a look in the examples in demo-projects/ to see how you can start your first check.

## Acrolinx Windows SDK

### [Getting Started with Acrolinx Windows SDK](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/2d2bad1b/windows-sdk/html/index.html)

## How Do I Get the SDKs?

Please contact [Acrolinx SDK support](https://github.com/acrolinx/acrolinx-coding-guidance/blob/master/topics/sdk-support.md).
On request, we'll upload the packages to your [Acrolinx download area](https://download.acrolinx.com/).

## License

Copyright 2015-present Acrolinx GmbH

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at:

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

For more information visit: [http://www.acrolinx.com](http://www.acrolinx.com)