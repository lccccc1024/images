# images

[闲话](https://blog.950922.xyz/) 博客的图片仓储，由 PicGo 自动上传，**不包含代码**。

## 用途

博客文章里的配图都存放在这里，仓库即图床，通过 jsDelivr CDN 对外提供访问，
不占用博客仓库的体积。

## 引用方式

```
https://cdn.jsdelivr.net/gh/lccccc1024/images/<文件名>
```

例如：

```markdown
![示例](https://cdn.jsdelivr.net/gh/lccccc1024/images/20250618101549.png)
```

也可以省略 `gh/` 段，用 `https://cdn.jsdelivr.net/gh/lccccc1024/images@main/<文件名>`
指定分支（`@main` 可换成任意 tag / commit）。

## 上传流程

1. 在 Typora / 编辑器里粘贴图片
2. PicGo 自动上传到本仓库并返回 jsDelivr 链接
3. 正文里插入的就是 CDN 地址

配置方式见博客文章：[使用 GitHub+PicGo 搭建免费图床](https://blog.950922.xyz/posts/2025-04-25-使用githubpicgo搭建免费图床/)

## 命名约定

- 平铺存放，不建子目录
- 文件名：时间戳（如 `20250618101549.png`）或短编号（`01.png` … `08.png`）

## 注意

- **不要删除或改名已引用的图片**，历史文章会立刻裂图
- jsDelivr 有边缘缓存，替换同名文件后短时间内可能仍返回旧图；
  需要立即生效时请改名或换新文件名
- 单文件建议控制在 1 MB 以内，仓库体积过大会拖慢 CDN 首次回源
