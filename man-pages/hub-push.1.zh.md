
# hub‐push(1)  ‐‐  Push a git branch to each of the listed remotes.

## SYNOPSIS

集线器推送<REMOTE>[,<REMOTE2>…][<ref>]

## EXAMPLES

```
$ hub push origin,staging,qa bert_timeout
> git push origin bert_timeout
> git push staging bert_timeout
> git push qa bert_timeout

$ hub push origin
> git push origin HEAD
```

## SEE ALSO

集线器(1),Git -Press(1)
