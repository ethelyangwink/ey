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
