
# hub‐pr(1) ‐‐ Manage GitHub pull requests for the current project.

## SYNOPSIS

"轮毂PR"列表[的S<STATE>][‐h <head>] [乙<BASE>]o \< SotTyKIK>[^ ]]  [f<FORMAT>][‐l <limit>]"轮毂PR"签出\< PR号码>[<BRANCH>]

## COMMANDS

-   *列表*列出当前项目中的拉取请求.

-   *结帐*在一个新的分支中检查拉取请求的头部.

## OPTIONS

-   s,s态<STATE>过滤器拉动请求<STATE>(默认:"打开").

-   H,头[<OWNER>:]<BRANCH>显示从指定的头部开始的拉取请求<BRANCH>. 默认值为<OWNER>从当前存储库中获取.

-   b,基<BRANCH>显示基于指定的拉取请求<BRANCH>.

-   f,格式<FORMAT>使用格式打印拉请求列表<FORMAT>(默认值:%SC%>(8)%i %cReal%t%%%n).请参阅git日志手册的"PRETTY FORMATS"部分,了解有关占位符如何以格式使用的更多细节.可用占位符是:

    ```
    %I: pull request number

    %i: pull request number prefixed with "#"

    %U: the URL of this pull request

    %S: state (i.e. "open", "closed")

    %sC: set color to red or green,  depending	on  pull  request
    ```

    状态.

    ```
    %t: title

    %l: colored labels

    %L: raw, comma‐separated labels

    %b: body

    %B: base branch

    %H: head branch

    %au: login name of author

    %as: comma‐separated list of assignees

    %Mn: milestone number

    %Mt: milestone title

    %NC: number of comments

    %Nc:  number  of  comments	wrapped  in parentheses, or blank
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

-   o,排序> \< SoTyKEKE>:按"创建"(默认)、"更新"、"流行"或"长时间运行"排序显示问题.

-   升排序:按升序排序而不是降序排序.

-   l、极限<LIMIT>只显示第一个<LIMIT>问题.

## SEE ALSO

轮毂问题(1),轮毂牵引请求(1),轮毂(1)
