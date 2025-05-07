# Contributing to CozyUI Ex

Thank you for your interest in contributing to **CozyUI Ex** project! Every contribution you make means a lot to us.

If you're a new contributor, please read this document to clarify the considerations you need to take into account when contributing to the project.

## Table of Contents

- [**Submit a mod support request or raise a resource pack bug.**](#submit-a-mod-support-request-or-raise-a-resource-pack-bug)
  - [What should I do?](#what-should-i-do)

- [**Participate in making.**](#participate-in-making)
  - [Getting Started.](#getting-started)
  - [Making textures.](#making-textures)
  - [Test.](#test)
  - [Pull request.](#pull-request)

- [**Publicizing the project.**](#publicizing-the-project)
- [**Styleguides.**](#styleguides)
  - [Commit messages.](#commit-messages)
  - [Files](#files)
- [**FAQ**](#faq)



## Submit a mod support request or raise a resource pack bug.

For this type of contribution, please go to the [Issues page](https://github.com/WhatDamon/cozyui-ex/issues) and submit a new issue.

We don't like a lot of duplicate issues piling up, so for every issue you submit, we expect you to check for duplicates as mentioned in the template.

### What should I do?

We use GitHub issues to track bugs and errors.

Before starting an issue submission, please update **CozyUI Ex** to the latest version, and for **CozyUI+**, please prioritize the recommended version and adjust the loading order as specified.

If the problem persists, open a new issue in the following order...

- Open an new [issue](https://github.com/WhatDamon/cozyui-ex/issues/new).
- Choose a template according to your requirements.
- Provide information according to the template.

## Participate in making.

> ### Legal Notice
> 
> When contributing to this project, you must agree that you have authored 100% of the content, that you have the necessary rights to the content and that the content you contribute may be provided under the project licence.
>
> This project uses the `GPLv3 license`, please read [this document](https://github.com/WhatDamon/cozyui-ex/blob/main/LICENSE) to clarify your rights and obligations!

In general, unless recognized by the author of this resource pack and given permissions, it is necessary to contribute the project via pull requests.

### Getting started.

Please run ...

~~~ bash
git clone https://github.com/Fogg05/CozyUI-Plus
~~~

to clone the original CozyUI+ repository. You can also use assets from CozyUI+ or CozyUI Ex resource packs.

and then run...

~~~bash
git clone https://github.com/WhatDamon/cozyui-ex
~~~

to clone CozyUI Ex repository. 

### Making textures.

Typically, CozyUI's texture size is 3 to 4 times of the original, if you want to make animation you need a `mcmeta` file and lengthen the texture image file vertically, you only need to use Photoshop to edit with the available textures.

You may be looking for requirements to create a split UI, or a one-piece UI, allow additional coloring as well, but usually Inventory uses the original gray.

More on creating a resource pack: https://minecraft.wiki/w/Tutorial:Creating_a_resource_pack

### Test.

After exporting the image and placing it in the corresponding location, load the resource pack and open the corresponding user interface to see if there is any problem.

### Pull request.

Please [fork this repository](https://github.com/WhatDamon/cozyui-ex/fork) before pulling the request, you need to commit your changes to the forked repository, after making sure it's done, please follow the steps below...

- Open a new [pull request](https://github.com/WhatDamon/cozyui-ex/compare).
- Follow the guide to complete the creation of a new pull request.

Project owners, as well as those involved, will make an assessment and decide whether or not to merge.

### Join us.

If you would like to participate in the production of this project on an ongoing basis, please send an email to [whatdamon@damon.top](mailto:whatdamon@damon.top).

Please describe in detail your reason for joining and include your GitHub account name in the email, and please use either English or Chinese to make your request, otherwise it will not be accepted.

If your request is approved, you will receive an invitation email from GitHub.

## Publicizing the project.

Feel free to publicize the project. However, during the process, we recommend pairing it with the CozyUI+!

## Styleguides.

To keep the project neat and maintainable, please observe the following styleguides!

### Commit messages.

Please observe the following rules for each commit message:

~~~
[TYPE]: [MESSAGE]
~~~

or...

~~~ 
[TYPE]([MODNAME]): [MESSAGE]
~~~

| **[TYPE]** | Descriptions                                                 |
| ---------- | ------------------------------------------------------------ |
| `feat`     | Add new mod user interface                                   |
| `fix`      | Fix some problems with existing textures, or just modified textures |
| `docs`     | Modification of documents                                    |
| `revert`   | Rolling back past commits                                    |
| `workflow` | Changes to Github Actions or production workflows            |
| `chore`    | Others                                                       |

**[MODNAME]**: The name (or namespace) of the target mod. *(optional)*

**[MESSAGE]:** Description of the modification.

### **Files**

Please observe the following file storage structure to ensure the maintainability of the repository.

~~~
cozyui-ex /
├── .github /
├── gallery /
├── pack /
│   ├── assets / <--- What you should modify
│   │   └── [MODNAMESPACE] /
│   │       └── textures/
│   │           └── gui /
│   │               ├── xxx.png <--- Image that will be loaded
│   │               └── xxx.png.mcmeta <--- Optional
│   ├── pack.mcmeta
│   └── pack.png
├── project /  <--- What you should modify
│   ├── [MODNAMESPACE] /
│   │   └── textures /
│   │       └── gui /
│   │           └── xxx.psd <--- Photoshop Project File
│   ├── background.png
│   └── pack.psd
├── CONTRIBUTING.md
├── LICENSE
└── README.md
~~~

## FAQ

Q: Can I use software like paint.net to edit or create textures?

*A: Yes, but you need to make sure that you have converted the project files to PSD files and that you have kept the layers!*
