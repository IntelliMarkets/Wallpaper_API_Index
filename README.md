<div align="center">

# <image src="https://github.com/user-attachments/assets/3b85e1ef-35e3-4f95-bf5e-90ca7f8fae13" height="45"/>  壁纸生成器 - 图片源市场
 <img src="https://img.shields.io/badge/FREE-100%25-brightgreen" alt="FREE">
<img src="https://img.shields.io/badge/Language-Python-blue" alt="Language">
<img alt="GitLab Stars" src="https://img.shields.io/github/stars/IntelliMarkets/Wallpaper_API_Index?label=Stars">

这里是 壁纸生成器 NEXT 的图片源市场，为壁纸生成器提供生成图片源的管理与更新功能。

[Main Repo](https://github.com/SRInternet-Studio/Wallpaper-generator/tree/NEXT-PREVIEW)

</div>

> [!Note]
>
> 📢**下架公告**：由于来自 i18.net 的图片源已经全部失效，经与用户讨论决定，官方于 2025.10.01 下架了来自 i18 接口的「CosPlay」, 二次元ACG」和「真人/动漫/风景」三个图片源
>
> ✨**上新公告**：经用户推荐、网络搜集，于 2025.11.01 上架了 1 个新图片源

## 编写指南
参见 **[APICORE 规范 1.0](https://github.com/SRON-org/APICORE/)**

## 如何上传
> [!Important]
> 
> **重要：请务必按照以下规范流程上传您的图片源配置文件，不规范的上传可能会导致无法正常在壁纸生成器中下载或更新你的图片源配置文件，还有可能导致图片源市场损坏。**
> 
> **对于造成图片源市场损坏的账户，我们将联系其并在一段时间内撤销其推送权限。**

1.  **Fork 本仓库**
    *   访问 [https://github.com/IntelliMarkets/Wallpaper_API_Index](https://github.com/IntelliMarkets/Wallpaper_API_Index/)。
    *   点击右上角的 "Fork" 按钮，将仓库复制到你的 GitHub 账号下。

2.  **克隆 (Clone) 你 Fork 的仓库到本地**
    *   在你的 GitHub 账号下找到你 Fork 的 Wallpaper_API_Index 仓库。
    *   点击 "Code" 按钮，复制仓库的 URL (以 `git@github.com` 或 `https://github.com` 开头)。
    *   打开你的终端 (Terminal) 或 Git Bash，执行以下命令：

        ```bash
        git clone <你复制的仓库 URL>
        cd Wallpaper_API_Index
        ```

3.  **（可选）创建图片源分类**
    *   在本地仓库的根目录下，创建一个文件夹，表示你的图片源所属的分类。**文件夹名称即代表你的分类名称**。 例如，如果你的图片源所生成的图片所属的分类为 "三次元"，则文件夹名称是 "三次元"。

        ```bash
        mkdir "三次元"
        ```
        
    *   当现有分类文件夹数量达到**4~5**个以上时，我们不是很推荐你创建一个新的分类，**过多的分类可能会造成图片源市场的混乱**。我们推荐你直接将你的图片源配置文件添加到现有分类中（参见步骤4），除非现有的分类确实不满足你的图片源所生成的图片类型。

4.  **将你的图片源配置文件 (*.json) 添加到分类**
    *   将你的图片源配置文件 (例如 `Pixiv.json`) 复制到表示分类的文件夹中。在添加之前，请检索本地仓库，查看是否已经存在同名的配置文件，我们不建议市场中存在完全同名的图片源。如果图片源相同但接口不同，你可以命名为 `*_n.json` (`n`表示数字，例如 `Pixiv_2.json`) 

5.  **提交 (Commit) 你的更改**
    *   在终端中，使用以下 Git 命令来暂存、提交你的更改：

        ```bash
        git add . 
        git commit -m "添加图片源：Pixiv" 
        ```

6.  **推送 (Push) 到你的 Fork 仓库**
    *   使用以下 Git 命令将本地更改推送到你 Fork 的 GitHub 仓库：

        ```bash
        git push origin main  # 推送到 origin 仓库的 main 分支 (如果你的仓库使用其他分支，请替换 main)
        ```

7.  **创建 Pull Request (PR)（重要）**
    *   访问你在 GitHub 账号下的 Fork 仓库。
    *   GitHub 会提示你 "Compare & pull request"，点击该按钮。
    *   填写 PR 的标题和描述信息，描述你添加了什么配置，以及图片源的描述。
    *   点击 "Create pull request" 按钮，提交你的 PR。

8.  **等待审核**
    *   仓库维护者会审核你的 PR，如果一切符合规范，你的图片源配置将被合并到主仓库中。

**仓库目录结构示例**

```
Wallpaper_API_Index/
├── 二次元/
│   ├── Pixiv.json
│   └── ...
└── 其他分类/
    ├── Other.json
    └── ...
```

**关于 Git 命令的补充说明：**

*   **`git clone`**:  将远程仓库复制到本地。
*   **`git add`**:  将文件添加到暂存区，准备提交。
    *   `git add .`  暂存所有更改。
    *   `git add <file_name>` 暂存指定文件。
*   **`git commit`**:  提交暂存区的更改，并添加描述信息。
*   **`git push`**:  将本地更改推送到远程仓库。
*   **`origin`**:  远程仓库的别名，通常指向你 Fork 的仓库。
*   **`main` (或 `master`)**:  分支名称，指定要推送到的分支。

至此，你已成功完成了图片源配置文件的上传。

<!-- 
> [!Warning]
> 
> 作为一名合格的开发者，你不应该开发具有成人色情、暴力、血腥等违反 GitHub 社区规定 的图片源上传至仓库，也不应改动别人的图片源文件夹。**一经审查发现有以上行为，将会被删除图片源，并在一段时间内撤销其推送权限。** -->

## 如何添加和删除图片源
1.	在壁纸生成器中打开图片源市场
2.	点击想要添加的图片源下的`添加`或`删除`按钮

## 关于
本文基于 [APICORE 规范 1.0](https://github.com/SRON-org/APICORE/) 编写。
