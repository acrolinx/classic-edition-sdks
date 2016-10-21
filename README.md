# Acrolinx Classic Edition SDKs

This document contains instructions and sample code to help developers integrate [Acrolinx](http://www.acrolinx.com/) in Java, .NET, or C++ applications. The SDKs take care of most of the functionality for you so you can develop integrations quickly.

## Automated or Authoring Integration

Acrolinx integrations serve 2 main use cases. 

### 1. Interactive, authoring integration

You can integrate Acrolinx in an authoring environment to give writers feedback while they edit content. For example, you might want to build an Acrolinx plug-in for a desktop XML editor.

### 2. Backend, automated integration

You can integrate Acrolinx in a server application to enable (automated) batch checking over a set of documents. For example, you might integrate Acrolinx in your CMS to check content as an automated workflow step.

## What is the difference between sidebar and classic edition?

Acrolinx plug-ins now come in [two different editions](https://support.acrolinx.com/hc/en-us/articles/208549775). 

The classic edition is the predecessor to the sidebar. With a classic edition plug-in, writers can check and edit their content with the help of a shortcut menu that appears when they click colored flags. 

The sidebar is the newest edition in the Acrolinx plug-in family. We've investe in this technology to provide a cross-platform SDK with a modern user experience. We've also simplified the API for integrators so you can build an Acrolinx integration by implementing a few methods and writing just a couple of lines of code. 

If you'd like to build an authoring integration, we strongly recommend using the Acrolinx sidebar.

See: [Recommendations](#recommendations)

## Prerequisites
Please contact Acrolinx SDK support (sdk-support@acrolinx.com) for consulting and getting your integration certified.

## Before you start

Check out our [Guidance for the Development of Acrolinx Integrations](https://github.com/acrolinx/acrolinx-coding-guidance).
Not all points might make sense your current project, or your company might have its own rules for writing code.
This document is designed to help you avoid common pitfalls when you develop an Acrolinx integration.

## Recommendations

### Develop an authoring integration

#### JavaScript
If you're developing a web-based Acrolinx integration, have a look at [Acrolinx Sidebar Demo](https://github.com/acrolinx/acrolinx-sidebar-demo).

#### .NET

See: [Acrolinx Sidebar .NET](https://github.com/acrolinx/acrolinx-sidebar-demo-dotnet)

#### You haven't found a sidebar SDK in your favorite coding language?

To run the [Sidebar](https://github.com/acrolinx/acrolinx-sidebar-demo) using your favorite coding language, you just need to load the sidebar in a web browser control and interact with the JavaScript inside.

Before you start building a new Acrolinx SDK on your own, contact Acrolinx SDK support (sdk-support@acrolinx.com). Chances are we're working on a sidebar SDK in the language you want to use...

### Develop a backend service integration

The standalone [Content Analyzer](https://support.acrolinx.com/hc/en-us/articles/211749485) might already sufficiently cover your use case for analyzing your content from an entire folder structure or website.

To run Acrolinx repeatedly as an automated task, you can use the [Command Line Checker](https://support.acrolinx.com/hc/en-us/articles/203943742).
The [Acrolinx Scorecard Analyzer project](https://github.com/acrolinx/acrolinx-scale#how-to-use-the-acrolinx-command-line-checker-to-perform-a-check) provides a script-based example of using the Command Line Checker. 

You can automatically run the Command Line Checker, for example, in a post-commit-hook of your source code repository like GIT, triggered by a continuous integration system like Jenkins, or run it by a task scheduler like cron or the Windows Task Scheduler.

The Acrolinx Java SDK is another option for using Acrolinx in a backend integration.

## Acrolinx Java SDK

[Getting Started with Acrolinx Java SDK Snippets](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/master/java-sdk/html/snippets.html)
[JavaDoc of Acrolinx JavaSDK](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/master/java-sdk/html/apidocs/index.html)


### The Acrolinx Java SDK in action - Starting the Demo Client

To see the Acrolinx Java SDK in action, execute the file `demo-projects/startable-swing-gui/java-sdk-gui-swing-sample.bat`.

#### To see the SWT Version of the Acrolinx Java SDK

1. Goto: `demo-projects/startable-swt-gui/`
2. Download correct SWT version depending on your environment: java vm + os from
[eclipse.org/swt](https://www.eclipse.org/swt/).
3. Extract the downloaded archive and copy the `swt.jar` to `demo-projects/startable-swt-gui/`
4. Start `java-sdk-gui-swt-sample.bat`

### First Steps with the Acrolinx Java SDK
1. Create a new java project
2. Copy the Acrolinx Java SDK jar into your project
3. Import this jar into the classpath of your new project
4. Take a look in the examples in demo-projects/ to see how you can start your first check.


## Acrolinx Windows SDK

## How do I get the SDKs?

Please contact Acrolinx SDK support (sdk-support@acrolinx.com). On request, we'll upload the packages to your [Acrolinx download area](https://download.acrolinx.com/).

## License

Copyright 2015-2016 Acrolinx GmbH

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

For more information visit: http://www.acrolinx.com
