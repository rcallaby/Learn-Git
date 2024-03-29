# Git 最佳实践和技巧
--
## 目录
- [管理干净的提交历史记录](#管理干净的提交历史记录)
  - [频繁且直观地提交](#频繁且直观地提交)
  - [编写描述性提交消息](#编写描述性提交消息)
  - [明智地使用分支](#明智地使用分支)
  - [变基以保持历史记录干净](#变基以保持历史记录干净)
  - [在推送之前压缩和编辑提交](#在推送之前压缩和编辑提交)
  - [避免直接推送到主分支](#避免直接推送到主分支)
  - [使用 Git Hooks](#使用GitHooks)
  - [文档更改和更新](#文档更改和更新)
  - [定期维护和清理](#定期维护和清理)
- [使用 Git 别名和快捷方式](#使用Git别名和快捷方式)
  - [了解Git别名](#了解Git别名)
  - [使用Git别名](#使用Git别名)
  - [共享Git 别名](#共享Git别名)
  - [在 GitHub 中使用 Git 别名](#在GitHub中使用Git别名)
- [使用.gitignore忽略文件和目录](#使用.gitignore忽略文件和目录)
  - [什么是.gitignore？](#什么是.gitignore？)
  - [创建 .gitignore](#创建.gitignore)
  - [.gitignore的语法](#.gitignore的语法)
  - [在 .gitignore 中使用模式](#在.gitignore中使用模式)
  - [.gitignore 的示例](#.gitignore的示例)
  - [全局 .gitignore](#全局.gitignore)
- [协作工作流和代码审查礼仪](#协作工作流和代码审查礼仪)
  - [Git 中的协作工作流](#Git中的协作工作流)
  - [代码审查礼仪](#代码审查礼仪)
  - [有效使用代码审查工具](#有效使用代码审查工具)
  - [在 GitHub 上协作](#在GitHub上协作)

---
## 管理干净的提交历史记录

像 Git 这样的版本控制系统和像 GitHub 这样的平台已经彻底改变了软件开发的管理和协作方式。有效使用 Git 和 GitHub 的一个重要方面是维护干净且有条理的提交历史记录。维护良好的提交历史记录不仅有助于开发人员更好地了解项目的演变，还有助于调试、代码审查和协作。在本文中，我们将探讨在 Git 和 GitHub 中管理干净提交历史记录的各种实践和技术。

### 频繁且直观地提交
频繁且合乎逻辑的提交是干净提交历史记录的基础。与其将大量更改捆绑到一个大规模提交中，不如进行表示逻辑工作单元的较小提交。理想情况下，每次提交都应解决一个特定问题、错误修复或功能。这种方法不仅有助于更好地理解，而且在必要时可以更轻松地还原更改。

### 编写描述性提交消息
A写得很好的提交消息对于理解提交引入的更改至关重要。避免使用“修复错误”或“更新代码”等通用提交消息。相反，请清晰简洁地描述更改及其背后的原因。提交消息应该采用命令式，使其读起来像命令或指令。例如：

好：“添加用户身份验证功能” 不理想：“添加了一些东西并修复了一些东西”

### 明智地使用分支
Git 中的分支是功能强大的工具，允许您在不影响主代码库的情况下处理单独的功能或错误修复。为您正在处理的每个新功能或问题创建一个新分支。这样，主分支（通常是 master 或 main）保持稳定，可以用作项目状态的基线。完成并测试分支上的工作后，使用干净且有据可查的合并提交将其合并回主分支。

### 变基以保持历史记录干净
Git 提供了一个称为“变基”的有用功能，它允许您将从一个分支的更改合并到另一个分支中，同时保持线性历史记录。使用 git rebase 将主分支中的更改集成到功能分支中，而不是合并分支，这可能会产生不必要的合并提交。变基有助于保持提交历史记录整洁且易于遵循。

### 在推送之前压缩和编辑提交
在将更改推送到 GitHub 等共享存储库之前，可以通过压缩和编辑提交来清理提交历史记录。使用 git rebase -i 以交互方式变基分支，并将多个提交合并为一个，或者编辑提交消息以清楚起见。压缩提交不仅可以减少混乱，还可以确保每次提交都代表一个连贯而完整的更改。

### 避免直接推送到主分支
在协作环境中，必须避免直接推送到主分支。相反，在 GitHub 等平台上使用拉取请求来提出更改，并让团队成员对其进行审查。这允许一种更有条理和更有条理的方法来将新代码集成到主分支中，同时保持提交历史记录的整洁。

### 使用GitHooks
Git hooks是可以在 Git 工作流中的某些点触发的脚本。利用预提交钩子来强制执行提交消息标准，或利用预推送钩子在将代码推送到远程存储库之前运行测试。这有助于保持一致性，并确保只推送干净且经过充分测试的更改。

### 文档更改和更新
除了清除提交消息外，还可以考虑维护项目的更改日志或发行说明。此文档可以包含在存储库的 README 或专用文件中。更新日志概述了每个版本引入的更改，使参与者和用户更容易了解新增功能和已修复的内容。

### 定期维护和清理
随着项目的发展，请花时间定期查看和清理提交历史记录。删除任何不必要或临时的分支，删除合并的分支，并考虑变基或压缩已过时或令人困惑的提交。

在 Git 和 GitHub 中，干净的提交历史记录不仅是一种最佳实践，而且是有效软件开发的一个重要方面。通过频繁提交、编写描述性提交消息、明智地使用分支以及利用 Git 的强大功能（如变基和压缩），开发人员可以维护有条理且有意义的提交历史记录。此外，合并 Git 钩子、记录更改和进行定期维护有助于确保项目在其整个生命周期中保持良好的结构和协作。

## 使用Git别名和快捷方式

Git 是一个强大的版本控制系统，被开发人员广泛用于管理源代码和项目协作。Git 的优势之一是它的灵活性和可定制性，它允许用户为常用命令创建别名和快捷方式。Git 别名和快捷方式可以显著提高工作效率，减少键入，并使 Git 命令更加直观。在本文中，我们将探讨如何设置和使用 Git 别名和快捷方式来增强 Git 和 GitHub 工作流程。

### 了解Git别名
Git 别名是 Git 命令的自定义快捷方式。它们允许您为复杂或常用的 Git 操作创建简单的缩写甚至全新的命令。Git 别名在 Git 配置文件 （.gitconfig） 中定义，该文件位于主目录 （~/.gitconfig） 或项目的根目录 （.git/config） 中。您可以设置应用于所有存储库的全局别名，也可以设置特定于特定项目的本地别名。

要创建 Git 别名，您可以使用 git config 命令或直接编辑 .gitconfig 文件。

创建全局 Git 别名： 要使用 git config 命令创建全局 Git 别名，请打开终端并输入：

```
git config --global alias.alias_name 'original_command'

```
将 alias_name 替换为所需的别名，original_command要缩短的完整 Git 命令。例如，要为 git status 创建别名，可以使用：

```
git config --global alias.st status

```
创建本地 Git 别名： 要为特定项目创建本地 Git 别名，请在终端中导航到该项目的根目录，并使用不带 --global 标志的相同 git config 命令：

```
git config alias.alias_name 'original_command'

```
### 使用Git别名
设置 Git 别名后，您可以立即开始使用它们。运行 Git 操作时，只需键入别名而不是完整命令即可。例如，如果您已经为 status 创建了 st 别名，您现在可以使用：

```
git st

```
这将为您提供与 git status 相同的结果。

#### 有用的 Git 别名示例：
以下是一些有用的 Git 别名示例，这些别名可以改进您的工作流程：

```
# Shortcuts for common commands
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.br branch

# Show abbreviated commit history
git config --global alias.lg "log --oneline --decorate --all --graph"

# Display colorful and more readable output for log
git config --global alias.l "log --pretty=format:'%C(auto)%h %Cblue%ad %Creset%s%C(auto)%d %Cgreen[%an]' --date=short"

# Show the current status of the repository
git config --global alias.s status

# View the commit history for a specific file
git config --global alias.filelog "log -u"

# Undo the last commit while keeping the changes
git config --global alias.undo "reset HEAD~1"

# Amend the last commit with staged changes
git config --global alias.amend "commit --amend --no-edit"


```
您可以根据自己的喜好和工作流程随意自定义这些别名。

### 共享Git别名
如果您在团队中或跨多台计算机工作，共享 Git 别名可能是有益的。您可以通过将相关条目从 .gitconfig 文件复制到队友或其他计算机的 .gitconfig 文件来共享别名。或者，您可以使用 git config 命令直接在这些计算机上设置别名。

要与他人共享您的别名，请向他们提供以下命令：

```
git config --global alias.alias_name 'original_command'

```
### 在GitHub中使用Git别名
Git 别名可与 GitHub 存储库无缝协作。无论是从 GitHub 存储库克隆、推送还是拉取，都可以像使用标准 Git 命令一样使用定义的别名。别名在计算机上本地应用，不会影响 GitHub 上托管的远程存储库。

对于任何使用 Git 和 GitHub 的开发人员来说，Git 别名和快捷方式都是一个有价值的工具。通过设置有意义且直观的别名，您可以显著提高工作效率，并使 Git 命令更易于记忆和使用。无论您是喜欢常用命令的简洁缩写，还是喜欢复杂操作的自定义快捷方式，Git 别名都允许您定制 Git 工作流程以满足您的需求。通过有效地使用和共享 Git 别名，您和您的团队可以简化开发过程并更高效地协作。

## 使用.gitignore忽略文件和目录

在软件开发中，版本控制对于管理源代码更改和与其他开发人员有效协作至关重要。Git 是最流行的版本控制系统之一，允许开发人员跟踪更改、创建分支和无缝合并代码。但是，并非 Git 应跟踪项目中的所有文件和目录。例如，生成项目、临时文件和敏感数据通常最好排除在版本控制之外。为此，Git 提供了一个简单而强大的解决方案：.gitignore 文件。在本文中，我们将探讨如何使用 .gitignore 将某些文件和目录排除在 Git 跟踪之外。

### 什么是.gitignore？
.gitignore 文件是一个纯文本文件，它告诉 Git 在暂存更改时要忽略哪些文件和目录。当您将文件或目录添加到 .gitignore 列表时，Git 会将它们排除在跟踪之外，这意味着它们不会出现在暂存区域中，并且对这些文件的后续更改不会记录在提交中。

### 创建.gitignore
若要开始使用 .gitignore，请在 Git 存储库的根目录下创建名为 .gitignore 的文件。您可以使用任何文本编辑器来创建此文件。请务必将文件命名为 .gitignore，不带任何文件扩展名。

例如，使用命令行，您可以创建如下所示的 .gitignore 文件：

```
touch .gitignore

```
### .gitignore的语法
.gitignore 文件使用简单的模式匹配来指定应忽略哪些文件和目录。基本语法规则如下：

空行或以 # 开头的行被视为注释，并被 Git 忽略。 要忽略特定文件，只需使用存储库根目录中的相对路径写入其名称即可。 若要忽略目录，请在末尾写一个尾部斜杠 （/） 的目录名称。

### 在.gitignore中使用模式
您可以在 .gitignore 中使用各种模式来指定要忽略的多个文件或目录。一些常用的模式包括：

通配符 （*）：匹配文件或目录名称中任意数量的字符。例如，.log 将忽略所有 .log 文件，build// 将忽略所有名为 build 的目录。

目录通配符 （）：匹配目录层次结构中任何级别的目录。例如，logs//*.log 将忽略日志的任何子目录中的所有 .log 文件。

否定 （！）：撤消以前的忽略规则。例如，如果要忽略所有 .txt 文件但保留一个文件，则可以使用 *.txt 忽略所有 .txt 文件，然后使用 ！important.txt 保留重要的 .txt。

### .gitignore的示例
以下是 .gitignore 条目的一些常见示例：

```
# Ignore build artifacts
build/
dist/
bin/

# Ignore log files
*.log

# Ignore temporary files
*.tmp
*.temp

# Ignore configuration files with sensitive data
config.ini
secrets.json

# Ignore files in a specific directory
data/*

# Ignore files with specific extensions
*.exe
*.dll


```
请记住，.gitignore 仅适用于未跟踪的文件。如果您在将文件添加到 .gitignore 之前已经跟踪了该文件，则将继续跟踪该文件。

### 全局.gitignore
有时，在多个 Git 存储库中，可能会忽略一些常见的模式。您可以设置一个适用于所有存储库的全局 .gitignore，而不是为每个存储库创建单独的 .gitignore 文件。

为此，请在主目录中创建一个全局 .gitignore 文件，并告诉 Git 将其用于所有存储库。请按照下列步骤操作：

创建全局 .gitignore 文件：

```
touch ~/.gitignore_global

```
使用与常规 .gitignore 文件相同的语法将忽略模式添加到全局文件。

告诉 Git 使用全局 .gitignore 文件：

```
git config --global core.excludesfile ~/.gitignore_global

```
使用 .gitignore 是有效管理 Git 存储库的一个基本方面。通过忽略不应跟踪的文件和目录，您可以保持存储库清洁，避免因不相关的更改而使版本历史记录混乱，并防止敏感数据被意外提交。.gitignore 文件是一个功能强大的工具，它允许您使用简单的模式匹配规则指定要排除的文件和目录。无论您是在构建新项目还是在团队中协作，掌握 .gitignore 的使用无疑将增强您的 Git 工作流程，并有助于更有条理和更高效的开发过程。

## 协作工作流和代码审查礼仪

协作是现代软件开发的核心，像 Git 这样的版本控制系统，加上像 GitHub 这样的平台，彻底改变了开发人员的工作方式。有效的协作工作流程和代码审查礼仪对于维护高质量的代码库、培养积极的团队文化以及确保新功能和错误修复的无缝集成至关重要。在本文中，我们将探讨 Git 和 GitHub 中协作工作流和代码审查礼仪的关键要素。

### Git中的协作工作流
Git 提供了多种协作工作流，其中最受欢迎的两个是集中式工作流和功能分支工作流。

集中式工作流程： 在集中式工作流中，所有团队成员都直接在单个分支（通常是主分支或主分支）上工作。开发人员克隆存储库，在本地进行更改，然后将这些更改推送到中央存储库。这种方法很简单，适用于代码更改频率较低的小型团队或项目。

但是，集中式工作流缺乏功能开发的隔离性，这可能会导致冲突并阻碍并行开发。

功能分支工作流： 功能分支工作流更具可扩展性，适用于大型团队和项目。在此工作流中，每个新功能或错误修复都是在专用分支上开发的。开发人员为特定任务创建一个新分支，处理更改，然后在完成后将该分支合并回主分支。

功能分支工作流为功能开发提供隔离，减少冲突，并实现更好的代码评审实践。它鼓励开发人员独立工作，并有助于更好地将新代码集成到主分支中。

### 代码审查礼仪
代码审查是协作开发过程的关键部分。它有助于识别错误，提高代码质量，并确保遵循最佳实践。以下是一些基本的代码审查礼仪提示：

尊重和建设性： 请记住，代码审查是关于改进代码，而不是批评开发人员。以尊重和建设性的方式提供反馈。关注代码的质量、对标准的遵守和整体设计，而不是个人喜好。

了解上下文： 在提供反馈之前，请尝试了解更改的上下文。熟悉功能或 bug 修复的目标，以及任何相关的设计决策或约束。

### 有效使用代码审查工具：
利用 GitHub 或其他平台提供的代码审查工具。利用内联评论来查明具体问题并提出改进建议。避免大而压倒性的评论;相反，将它们分解为更小的、可操作的点。

解决高层次和低层次的问题： 提供有关整体体系结构、设计模式和代码组织等高级方面的反馈，以及变量名称、代码格式设置和错误处理等低级别详细信息的反馈。对这两个方面的关注有助于更全面的代码审查。

避免吹毛求疵： 虽然对细节的关注是必不可少的，但要避免吹毛求疵或过分关注不会对代码的功能或可维护性产生重大影响的小问题。

设定切合实际的时机期望： 考虑变更的紧迫性，并为审核时间设定切合实际的期望。较小和不太重要的更改可能需要更快的周转时间，而较大的更改或功能实现可能需要更多时间。

乐于接受反馈： 作为代码作者，请乐于接收反馈。将反馈视为成长和改进的机会，并准备好解决审稿人提出的问题。

使用自动检查和测试： 在启动代码审查之前，请运行自动检查和测试，以捕获常见问题，例如编码样式冲突和基本错误。这确保了审阅者在审阅过程中可以专注于更高层次的方面。

### 在GitHub上协作
GitHub 提供了许多协作功能来补充 Git 工作流程。协作开发的一些关键功能包括：

#### 拉取请求：
拉取请求 （PR） 是功能分支工作流的基石。当开发人员准备好将其功能分支合并到主分支时，他们会创建一个拉取请求。PR 提供更改的清晰概述，并允许团队成员在合并之前评论、建议更改和讨论代码，从而促进代码审查。

#### 代码审查请求：
创建拉取请求时，请请求特定团队成员查看更改。这确保了通知正确的人，并且审查过程是有效的。

#### 状态检查和持续集成 （CI）：
设置状态检查和 CI，以便在拉取请求中提出更改时自动运行测试和检查。这在将代码合并到主分支之前提供了额外的置信度。

#### 标签和里程碑：
使用标签和里程碑对拉取请求进行分类和跟踪。标签可以指示 PR 的状态（例如，“需要审查”、“正在进行的工作”），而里程碑可以对特定版本或功能的相关 PR 进行分组。

协作工作流和代码审查礼仪是使用 Git 和 GitHub 成功开发软件的基本方面。通过为您的团队采用正确的工作流（例如功能分支工作流），您可以确保更顺畅的并行开发并最大限度地减少冲突。有效的代码审查礼仪，包括建设性的反馈、理解上下文和有效地使用代码审查工具，可以培养积极的团队文化并提高代码质量。利用 GitHub 的协作功能，例如拉取请求、状态检查和里程碑，进一步简化开发流程并增强团队协作。通过将这些最佳实践整合到您的工作流程中，您可以实现更有条理、更高效和更具协作性的软件开发流程。
