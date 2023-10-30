# 贡献准则
感谢您考虑为 Learn-Git 做出贡献！这个存储库旨在为正在学习 Git 的人提供资源，你的贡献可以帮助它变得更好。

如果您想通过改进本教程或可能将其翻译成另一种语言来为该存储库做出贡献，请使用该想法或改进创建一个新问题，如果该想法足够好，我或该存储库的潜在成员将批准它。此时，您可以创建更改，然后创建拉取请求。

## 行为准则
在开始之前，请阅读并遵守行为准则。我们希望为所有参与者保持一个尊重和热情的社区。

## 开始
以下是为 Learn-Git 做贡献的基本步骤：

- **分叉存储库**

![fork_image](./images/Readme_images/fork.png)

- **为更改创建新分支**

```
git branch "branch-name"
```
### 参考图片
![branch_image](./images/Contributing_images/branch_making.png)

然后使用以下语法打开该分支：

### 语法
```
git checkout "branch-name"
```

### 参考图片
![checkout_branch](./images/Contributing_images/checkout_image.png)


- **进行更改并将其提交到分支**

在进行任何更改或添加后，在终端中使用此命令
```
git add .
```
提交更改或添加的语法

```
git commit -m "A brief description of the changes made"
```

### 参考图片
![commiting_images](./images/Contributing_images/add_commit.png)

- **将更改推送到分支**

将更改推送到 GitHub：将更改提交到本地存储库后，需要将其推送到 GitHub。这将使用您所做的更改更新 GitHub 帐户中存储库的副本。若要推送更改，请使用以下命令：

```
git push origin branch-name

```
### 参考图片
![Push](./images/Contributing_images/push_origin.png)

- **创建拉取请求**

将更改推送到 GitHub 后，当您重新加载分叉的存储库时，您将看到创建拉取请求的选项。单击该按钮以创建拉取请求。

### 参考图片

![Pull Request](./images/Contributing_images/pull_request.png)

这将带你进入一个页面，您可以在其中查看所做的更改并提供拉取请求的描述。

请务必清晰简洁地描述您所做的更改以及您进行更改的原因。

如果存储库所有者应该注意任何问题或疑虑，请务必在拉取请求描述中提及它们。

对描述感到满意后，单击“创建拉取请求”按钮。

![Last Image](./images/Contributing_images/last.png)

等待反馈：创建拉取请求后，存储库所有者将查看您的更改并提供反馈。

## 如何贡献
我们欢迎以下形式的投稿：

### 修正
如果您在现有内容中发现任何错误或不准确之处，请提出问题，请详细描述错误或不准确之处。如果验证了这些错误或不准确之处的准确性，则可以打开包含这些更改的拉取请求。请尝试勤奋并将问题链接到您的拉取请求。另请记住，个人对语法的偏好并不一定构成必要的更改。

### 增加
如果你对新内容有想法，你认为对学习 Git 的人很有价值，请先打开一个问题来讨论它。获得批准后，请随时使用您的新内容创建拉取请求。

### 改进
如果您有改进现有内容的建议，请先打开一个问题进行讨论。获得批准后，请随时创建包含改进的拉取请求。

## 风格指南
在为 Learn-Git 做贡献时，请遵循以下风格指南：

- 使用简洁明了的语言
- 使用标题和副标题来分解部分
- 使用示例和视觉对象来说明概念
- 在适当的时候包括相关资源的链接
- 使用美式英语拼写和语法

# 总结
感谢您抽出宝贵时间为 Learn-Git 做出贡献！你的贡献可以帮助刚入门的人更容易访问 Git。
