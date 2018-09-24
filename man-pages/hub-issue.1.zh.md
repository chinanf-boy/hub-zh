# hub‐issue(1) ‐‐ Manage GitHub issues for the current project.

## SYNOPSIS

"枢纽问题"[A<ASSIGNEE>][‐c <creator>] ["@"<USER>][‐s <state>] [f<FORMAT>][‐m <milestone>] [l<LABELS>][‐d <date>]
[o \< SORTTKEY > > \[^ ^ \]][‐l <limit>]"hub 发行"[英国石油公司][‐m <message>|‐f <file>] [编辑][‐a <users>] [米<MILESTONE>][‐l <labels>]"hub 发行"标签[彩色]

## 命令

没有参数,显示一个公开问题的列表.

- *创造*打开当前项目中的一个问题.

- *标签*列出这个存储库中可用的标签.

## OPTIONS

- A、受让人<ASSIGNEE>只显示分配给的问题<ASSIGNEE>.

  ```
  When opening an issue, this can be a comma‐separated list  of
  ```

  人们分配给新的问题.

- C,创造者<CREATOR>只显示由问题创建的问题<CREATOR>.

- "@"、"提到"<USER>只显示问题<USER>.

- s,s 态<STATE>显示状态问题<STATE>(默认:"打开").

- f,格式<FORMAT>使用格式打印问题的内容<FORMAT>(默认值:%SC%>(8)%i %cReal%t%%%n).请参阅 git 日志手册的"PRETTY FORMATS"部分,了解有关占位符如何以格式使用的更多细节.问题的可用占位符是:

  ```
  %I: issue number

  %i: issue number prefixed with "#"

  %U: the URL of this issue

  %S: state (i.e. "open", "closed")

  %sC: set color to red or green, depending on issue state.

  %t: title

  %l: colored labels

  %L: raw, comma‐separated labels

  %b: body

  %au: login name of author

  %as: comma‐separated list of assignees

  %Mn: milestone number

  %Mt: milestone title

  %NC: number of comments

  %Nc: number of comments  wrapped  in  parentheses,	or  blank
  ```

  字符串为零.

  ```
  %cD: created date‐only (no time of day)

  %cr: created date, relative

  %ct: created date, UNIX timestamp

  %cI: created date, ISO 8601 format

  %uD: updated date‐only (no time of day)

  %ur: updated date, relative

  %ut: updated date, UNIX timestamp

  %uI: updated date, ISO 8601 format
  ```

- M,消息<MESSAGE>使用第一行<MESSAGE>作为标题,其余的作为问题描述.

- f,文件<FILE>阅读问题标题和描述<FILE>.

- e,编辑:进一步编辑内容<FILE>在提交之前的文本编辑器中.

- o,浏览:在 Web 浏览器中打开新的问题.

- c,拷贝:把新问题的 URL 放在剪贴板上,而不是打印它.

- m,里程碑<ID>只显示带有 GID 的 Github 里程碑的问题<ID>.

  ```
  When opening an issue, add this issue to a	GitHub	milestone
  ```

  带身份证<ID>.

- L,标签<LABELS>只显示带有某些标签的问题.

  ```
  When  opening  an issue, add a comma‐separated list of labels
  ```

  对此问题.

- d,此后<DATE>只显示更新后或更新后的问题<DATE>采用 ISO 8601 格式.

- o,排序> \< SoTyKEKE>:按"创建"(默认)、"更新"或"注释"排序问题.

- 升排序:按升序排序而不是降序排序.

- l、极限<LIMIT>只显示第一个<LIMIT>问题.

- 包括牵线:包括拉请求以及问题.

- 颜色:为标签列表启用彩色输出.
