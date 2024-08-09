# Overview

Cerebellum is a scaleable, open-source, drop-in infrastructure for realtime applications. That's a mouthful! 

In short: **we help you ship WebSocket-based realtime applications faster and more reliably**.

To learn more about Cerebellum's development in detail, read our case study [here](https://docs.google.com/document/d/1WC1yrta0Rao3_08TVQburuwODeZ3hy00GHWGn716NXE/edit).

## At a Glance

Cerebellum is made up of several tools. Take a look at their READMEs, linked below:
- [CLI](https://github.com/Cerebellum-Realtime/cli): deploy Cerebellum's infrastructure in just a few clicks
- [Client Library](https://github.com/Cerebellum-Realtime/clientLibrary): interact with Cerebellum on the front end
- [CDK](https://github.com/Cerebellum-Realtime/cdk): provision the AWS infrastructure that makes up Cerebellum
- [Server](https://github.com/Cerebellum-Realtime/server): manage the back-end server that powers Cerebellum

To take a look at some examples/code samples from applications built with Cerebellum, take a look at:
- [Realtime chat application](https://github.com/Cerebellum-Realtime/sample_app)
- [Realtime collaborative editor](https://github.com/Cerebellum-Realtime/collabEditor)

## Getting Started
### Prerequisites

To create a Cerebellum application, the following must be installed/configured:
- Node.js
- AWS (see Cerebellum CLI for details)
- React (if using Cerebellum React hooks)

Once you have these dependencies installed, you can use the Cerebellum CLI tool to create a Cerebellum application. Learn more about the CLI tool [here](https://github.com/Cerebellum-Realtime/cli).
- `npm install -g @cerebellum/cli` to install the Cerebellum CLI tool
- `cerebellum --help` to view a few useful commands for creating Cerebellum applications

### Your First Cerebellum Application
There are two options for creating Cerebellum applications:
- `cerebellum create` to create a new directory and deploy Cerebellum's infrastructure to AWS
- `cerebellum init` to deploy Cerebellum's infrastructure in the current directory

Either of these commands will spin up an infrastructure that is configured to meet the specific needs of realtime applications. Cerebellum provides a preconfigured [WebSocket server](https://github.com/Cerebellum-Realtime/server) out of the box. You can use the [Cerebellum Client Library](https://github.com/Cerebellum-Realtime/clientLibrary) to interact with our server, or you can bring your own WebSocket server and only use Cerebellum for its infrastructure.

Once the Cerebellum infrastructure deployment is complete, you can get started developing right away.
- Create a React or vanilla JavaScript application to power your front end
- `npm install @cerebellum/sdk` to install the Cerebellum Client Library
- `npx cerebellum-start` to run the Cerebellum Docker image and dependencies for local development

Now you can start developing with Cerebellum!

### Spinning Down
If at any point you want to stop the local development environment:
- `npx cerebellum-stop`

To delete the Cerebellum infrastructure:
- `cerebellum destroy`

#### Meet the Founders
Cerebellum was built by a group of four software engineers with a passion for coding and realtime applications. Together, we cover three of the four major cities in Texas—Dallas, Houston, and Austin—as well as one Canadian based out of Toronto. Our Canadian team member has since become an expert in the use of "y'all" and the mecca of "gastinations," Buc-ee's. In return, he has educated the Texan members on the benefits of poutine, maple syrup, and Tim Hortons.

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
