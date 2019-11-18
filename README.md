# DEPRECATED Acrolinx Classic Integration SDKs

The following instructions and sample code will help you integrate [Acrolinx](https://www.acrolinx.com/)
in Java, .NET, or C++ applications.
The SDKs take care of most of the functionality for you, so you can develop integrations quickly.

## New Acrolinx Platform API

Don't build new projects based on the Classic API. The Classic API is sun set. See: [Product Sunset Policy](https://docs.acrolinx.com/coreplatform/latest/en/compatibility/product-sunset-policy).
This documentation is only for maintaining existing projects.
Acrolinx released a new [Platform API](https://github.com/acrolinx/platform-api) with version 2018.12.
Several SDKs automated as well as Sidebar SDKs are available on GitHub.

## Prerequisites

Please contact [Acrolinx SDK support](https://github.com/acrolinx/acrolinx-coding-guidance/blob/master/topics/sdk-support.md)
for consulting and getting your integration certified.
This sample works with a test license on an internal Acrolinx URL.
This license is only meant for demonstration and developing purposes.
Once you finished your integration, you'll have to get a license for your integration from Acrolinx.
  
Acrolinx offers different other SDKs, and examples for developing integrations.

Before you start developing your own integration, you might benefit from looking into:

* [Getting Started with Custom Integrations](https://docs.acrolinx.com/customintegrations),
* the [Guidance for the Development of Acrolinx Integrations](https://github.com/acrolinx/acrolinx-coding-guidance),
* the [Acrolinx SDKs](https://github.com/acrolinx?q=sdk), and
* the [Acrolinx Demo Projects](https://github.com/acrolinx?q=demo).

## Automated or Authoring Integration

Acrolinx Integrations serve two main use cases.

### 1. Interactive, Authoring Integration

You can integrate Acrolinx in an authoring environment to give writers feedback while they edit content.
For example, you might want to build an Acrolinx Integration for a desktop XML editor.

### 2. Embedded Integration

You can integrate Acrolinx in a server application to enable (automated) batch checking over a set of documents.
For example, you might integrate Acrolinx in your CMS to check content as an automated workflow step.

## Difference Between Sidebar and Classic Integration

Acrolinx Integrations now come in [two different editions](https://support.acrolinx.com/hc/en-us/articles/208549775).

The Classic Integration is the predecessor to the Sidebar. With a Classic Integration integration,
writers can check their content. They can edit with the help of a shortcut menu that appears when they click colored issues.

The Sidebar is the newest edition in the Acrolinx Integration family.
We've invested in this technology to provide a cross-platform SDK with a modern user experience.
We've also simplified the API for integrators. You can build an Acrolinx Integration by implementing a few methods
and writing just a couple of lines of code.

If you'd like to build an authoring integration, we strongly recommend using the Acrolinx Sidebar.

See: [Recommendations](#recommendations)

## Recommendations

### Develop an Authoring Integration

#### JavaScript

If you're developing a web-based Acrolinx Integration, have a look at [Acrolinx Sidebar Demo](https://github.com/acrolinx/acrolinx-sidebar-demo).

#### .NET

See: [Acrolinx Sidebar .NET](https://github.com/acrolinx/acrolinx-sidebar-demo-dotnet)

#### C++

See: [Acrolinx Sidebar C++](https://github.com/acrolinx/sidebar-demo-cpp)

#### Java

See: [Acrolinx Sidebar Java](https://github.com/acrolinx/acrolinx-sidebar-demo-java)

#### Other Coding Languages

You haven't found a Sidebar SDK in your favorite coding language?

To run the [Sidebar](https://github.com/acrolinx/acrolinx-sidebar-demo) using your favorite coding language,
you just need to load the Sidebar in a web browser control and interact with the JavaScript inside.

Before you start building a new Acrolinx SDK on your own, contact [Acrolinx SDK support](https://github.com/acrolinx/acrolinx-coding-guidance/blob/master/topics/sdk-support.md).
Chances are we're working on a Sidebar SDK in the language you want to use...

### Develop an Embedded Integration

The standalone [Content Analyzer](https://docs.acrolinx.com/ca/latest/en)
might already sufficiently cover your use case for analyzing your content from an entire folder structure or website.

To run Acrolinx repeatedly as an automated task, you can use the [Acrolinx Command Line Interface](https://docs.acrolinx.com/cli/latest/en).

You can automatically run the Command Line Interface. For example,
in a post-commit-hook of your source code repository. That could be GIT, started by a continuous integration system like Jenkins,
or run it by a task scheduler like cron or the Windows Task Scheduler.

The Acrolinx Java SDK is another option for using Acrolinx in an embedded integration.

## Acrolinx Java SDK

### [Getting Started with Acrolinx Java SDK Snippets](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/5750a55d31d0d5fe267e75c768660f5f7d42c606/java-sdk/html/snippets.html)

### [JavaDoc of Acrolinx Java SDK](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/5750a55d31d0d5fe267e75c768660f5f7d42c606/java-sdk/html/apidocs/index.html)

### Starting the Demo

To see the Acrolinx Java SDK in action, execute the file `demo-projects/startable-swing-gui/java-sdk-gui-swing-sample.bat`.

#### Acrolinx Java SDK SWT Demo

1. Goto: `demo-projects/startable-swt-gui/`
2. Download correct SWT version depending on your environment: java VM + os from [eclipse.org/swt](https://www.eclipse.org/swt/).
3. Extract the downloaded archive and copy the `swt.jar` to `demo-projects/startable-swt-gui/`
4. Start `java-sdk-gui-swt-sample.bat`

### First Steps with the Acrolinx Java SDK

1. Create a new java project
2. Copy the Acrolinx Java SDK jar into your project
3. Import this jar into the classpath of your new project
4. Take a look in the examples in `demo-projects/` to see how you can start your first check.

## Acrolinx Windows SDK

### [Getting Started with Acrolinx Windows SDK](https://cdn.rawgit.com/acrolinx/classic-edition-sdks/2d2bad1b/windows-sdk/html/index.html)

## How Do I Get the SDKs?

Please contact [Acrolinx SDK support](https://github.com/acrolinx/acrolinx-coding-guidance/blob/master/topics/sdk-support.md).
On request, we'll upload the packages to your [Acrolinx Download Area](https://download.acrolinx.com/).

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

For more information visit: [https://www.acrolinx.com](https://www.acrolinx.com)