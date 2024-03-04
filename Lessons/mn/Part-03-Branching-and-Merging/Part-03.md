# Branch(салаа) үүсгэх ба Merge хийх(нэгтгэх)

- [Branch ба түүний зорилго](#branch-ба-түүний-зорилго)
- [Branch үүсгэх болон тэдний дунд шилжих](#branch-үүсгэх-болон-тэдний-дунд-шилжих)
- [Branch-н түүхийг удирдах ба өөрчлөлтүүдийг нэгтгэх (merge)](<#branch-ийн-түүхийг-удирдах-ба-өөрчлөлтүүдийг-нэгтгэх-(merge)>)
- [Нэгтгэлийн зөрчилдөөнийг(merge conflicts) зохицуулах](<#нэгтгэлийн-зөрчилдөөнийг(merge-conflicts)-зохицуулах>)
- [Дүгнэлт](#дүгнэлт)

# Branch ба түүний зорилго:

Программ хөгжүүлэлтийн хүрээнд Git branch нь хамтран ажиллах, кодын өөрчлөлтийг удирдахад зайлшгүй хэрэгтэй "багаж" юм. Git-д branch гэдэг нь ерөнхийдөө repository-н commit түүхийн тодорхой нэг commit руу заасан хөнгөн, хөдөлгөх боломжтой заагч сум юм. Branch-г ашигласнаар хөгжүүлэгчид нэг төслийн өөр өөр хэсэгт нэгэн зэрэг ажиллаж, шинэ функциональ турших эсвэл засах болон үндсэн кодын санд нөлөөлөхгүйгээр өөрчлөлтүүдийг тусгаарлаж болно. Энэ нийтлэл Git branch-ын нарийн ширийнийг судалж, хэрхэн үүсгэх, шилжих, түүх удирдах, merge-н зөрчилдөөнийг зохицуулах талаар үзнэ.

### Branch үүсгэх болон тэдний дунд шилжих:

To create a new branch in Git, developers can use the "git branch" command, followed by the desired branch name. For example, to create a branch named "feature-branch," one would execute the command: git branch feature-branch. This creates a new branch, but the repository's HEAD (the currently active branch) remains unchanged. An example is given here:

```bash
git branch feature-branch
```

To switch to the newly created branch, the "git checkout" command is employed. By typing git checkout feature-branch, the HEAD will be updated, and the developer will be working within the "feature-branch" context. An example would be:

```bash
git checkout feature-branch
```

Alternatively, Git 2.23 introduced a more convenient way to create and switch to a new branch in a single step: git checkout -b feature-branch. This command creates the branch and switches to it simultaneously. Such as:

```bash
git checkout -b feature-branch
```

### Branch-ийн түүхийг удирдах ба өөрчлөлтүүдийг нэгтгэх (merge):

Branches serve as isolated environments where developers can work on specific features or bug fixes. While on a branch, developers can make changes, commit them, and build up the branch's commit history independently of the main branch or other branches.

When changes on a branch are complete and ready for integration, merging comes into play. Merging is the process of combining the changes made in one branch into another. To merge the changes from a branch (e.g., "feature-branch") into the main branch, developers can execute the command git merge feature-branch while on the main branch. This action integrates the changes from "feature-branch" into the main branch, combining commit histories.

<img alt="Git branching and merging infographic" src="../../../images/Part-03/branching-and-merging.png" />

### Нэгтгэлийн зөрчилдөөнийг(merge conflicts) зохицуулах:

Merge conflicts occur when Git encounters conflicting changes between the source branch (e.g., "feature-branch") and the target branch (e.g., main branch) during a merge operation. Conflicts typically arise when the same lines of code have been modified in different ways on the two branches.

To address merge conflicts, developers need to manually resolve the conflicting lines. Git provides markers within the conflicting file, indicating the conflicting sections, and developers must edit the file to select the desired changes. After manually resolving the conflicts, developers save the file and complete the merge by adding and committing the changes. Git marks the conflict as resolved and completes the merge operation.

In cases where conflicts prove challenging to resolve, developers can seek assistance from Git's merge tools or collaborate with team members to find suitable resolutions.

# Дүгнэлт:

Git branches are indispensable tools for managing code evolution and facilitating collaboration in software development. By utilizing branches, developers can work on different features or bug fixes simultaneously, without impacting the main codebase. Branches allow for the independent development and isolation of changes, which can be merged into the main branch when ready.

With a clear understanding of branch creation, switching, history management, and conflict resolution, developers can effectively leverage Git branches to maintain a structured and efficient development process. By embracing Git branches, software development teams can enhance productivity, enable parallel work, and ultimately deliver high-quality code.
