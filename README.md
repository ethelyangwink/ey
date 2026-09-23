# ey

可安装的 Codex skills 集合，目前包含中文简历写作 skill。

## 安装

安装整个集合：

```bash
npx skills add ethelyangwink/ey
```

只安装简历写作 skill：

```bash
npx skills add ethelyangwink/ey --skill resume-writing
```

只安装剪视频 skill：

```bash
npx skills add ethelyangwink/ey --skill capcutmate-jianying-editing
```

安装后重新启动 Codex，会话即可识别新增 skill。

## 安装后提醒：如何找到 Word 简历模板

当要把简历的内容填到 Word 简历模板里时：

1. 先确定简历最终存放目录，优先使用用户明确提供的目录。
2. 在该目录中查找文件名包含“简历模板”的 `.docx` 或 `.doc` 文件。
3. 找到多个模板时，使用用户指定的版本；无法判断时请用户选择。
4. 找到模板后先复制成新的 `.docx` 工作文件，再填入简历内容，保留模板源文件不变。
5. 没有找到模板时，请用户提供模板路径或文件，不要创建空白模板替代。

## 当前包含

- `resume-writing`：先核对岗位与公司业务，再按用户意图控制中文简历的改写尺度。
- `capcutmate-jianying-editing`：中文口播视频精剪，覆盖重录清理、停顿处理、可编辑字幕和剪映草稿验收。

### 剪视频 skill 的首次使用

安装并重启 Codex 后，首次调用剪视频 skill 会先说明用法，并向用户确认以下路径：

```text
原始视频和图片素材保存目录：
剪映草稿工作区：
备份和中间文件目录：
导出目录（如需要）：
```

这些路径由用户指定或从当前项目明确识别，skill 不预设本机目录，也不会把素材写入 skill 安装目录。后续剪辑会沿用已经确认的项目路径；更换项目或路径发生变化时重新确认即可。原始素材保留在素材目录，剪映时间线只引用项目草稿工作区内经过确认的稳定文件，临时下载目录和缓存目录不作为长期引用来源。
