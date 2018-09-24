
Hub释放(1)管理GITHUB版本.= =

## SYNOPSIS

"毂释放"[包括草案][‐‐exclude‐prereleases]  [l<LIMIT>]"毂释放"秀<TAG>"毂释放"创建[DPOC][‐a <file>] [米<MESSAGE>f<FILE>][‐t <target>] <TAG>"轮毂重租"编辑[<options>] <TAG>"中枢释放"下载<TAG>"中枢释放"删除<TAG>

## COMMANDS

在没有参数的情况下,显示现有版本的列表.

有"包括草案",包括草案在上市.使用"排除排除",从列表中排除非稳定版本.

-   *显示*显示GITHUB发行说明<TAG>.

    使用"显示下载",包括"下载"部分.

-   *创造*创建指定的GITHUB版本<TAG>姓名.如果Git标签<TAG>不存在,它将在<TARGET>(默认:租金分支).

-   *编辑*编辑指定的GITHUB版本<TAG>姓名.接受相同的选项*创造*命令.用"草稿=虚报"发布草稿.

    ```
    When  <MESSAGE>  or  <FILE>  are not specified, a text editor
    ```

    将开放前填充当前发行的标题和身体.重新使用现有的标题和身体不变,通过"m".

-   *下载*下载指定版本的附加资产<TAG>.

-   *删除*删除指定的发行版和相关资产<TAG>.

## OPTIONS

-   l,限制:只显示第一个<LIMIT>释放.

-   D,草案:创建一个草案释放.

-   P,预存:创建预发布.

-   A,附加<FILE>在这个版本中附加一个文件作为一个资产.

    ```
    If	<FILE> is in the "<filename>#<text>" format, the text af‐
    ```

    将"γ"字符作为资产标签.

-   M,消息<MESSAGE>使用第一行<MESSAGE>作为发布标题,其余的作为发布说明.

-   f,文件<FILE>请阅读发布的标题和描述<FILE>.

-   e,编辑:进一步编辑内容<FILE>在提交之前的文本编辑器中.

-   o,浏览:在Web浏览器中打开新版本.

-   c,拷贝:把新版本的URL放在剪贴板上,而不是打印它.

-   公平交易<TARGET>一个提交SHAN或分支名称来附加释放,仅用于<TAG>还不存在(默认:主分支).

-   f,格式<FORMAT>使用漂亮的打印版本<FORMAT>(默认值:%t%n).请参阅Git -log(1)的"漂亮格式"部分,了解占位符如何在格式中使用的其他细节.问题的可用占位符是:

    ```
    %U: the URL of this release

    %uT: tarball URL

    %uZ: zipball URL

    %uA: asset upload URL

    %S: state (i.e. "draft", "pre‐release")

    %sC: set color to yellow or red, depending on state

    %t: release name

    %T: release tag

    %b: body

    %as: the list of assets attached to this release

    %cD: created date‐only (no time of day)

    %cr: created date, relative

    %ct: created date, UNIX timestamp

    %cI: created date, ISO 8601 format

    %pD: published date‐only (no time of day)

    %pr: published date, relative

    %pt: published date, UNIX timestamp

    %pI: published date, ISO 8601 format
    ```

-   <TAG>这个版本的Git标签名.

## SEE ALSO

集线器(1),GIT-TAG标签(1)
