# awesome-git-tools

List of useful Git tools

## Contents

- [Pager](#pagers)
- [Diffs](#diffs)
- [Conflict resolution](#conflict-resolution)
- [Merge](#merge)

## Pagers

| Name          | Homepage                             | Repository                                  | Performance | Speed    | Price | License    |
| ------------- | ------------------------------------ | ------------------------------------------- | ----------- | -------- | ----- | ---------- |
| bat           | -                                    | <https://github.com/sharkdp/bat>            | -           | Fastest  | Free  | Apache-2.0 |
| delta         | <https://dandavison.github.io/delta> | <https://github.com/dandavison/delta>       | -           | Fastest  | Free  | MIT        |
| diff-so-fancy | -                                    | <https://github.com/so-fancy/diff-so-fancy> | -           | Moderate | Free  | MIT        |
| diffr         | -                                    | <https://github.com/mookid/diffr>           | -           | Fastest  | Free  | MIT        |
| less          | -                                    | Built-in                                    | -           | Fast     | Free  | GPL-3.0    |

## Diffs

| Name         | Homepage                           | Repository                                  | Performance | Speed    | Price       | License      |
| ------------ | ---------------------------------- | ------------------------------------------- | ----------- | -------- | ----------- | ------------ |
| diffsitter   | -                                  | <https://github.com/afnanenayet/diffsitter> | Better      | Fastest  | Free        | MIT          |
| difftastic   | <https://difftastic.wilfred.me.uk> | <https://github.com/Wilfred/difftastic>     | Best        | Faster   | Free        | MIT          |
| Glim (macOS GUI) | - | <https://github.com/NeoPanic/Glim> | - | - | Free | MIT |
| GumTree      | -                                  | <https://github.com/GumTreeDiff/gumtree>    | -           | Moderate | Free        | LGPL-3.0     |
| icdiff       | <https://www.jefftk.com/icdiff>    | <https://github.com/jeffkaufman/icdiff>     | -           | Slow     | Free        | GPL-like ?   |
| sdiff        | -                                  | <https://github.com/pulkin/sdiff>           | Good        | Fast     | Free        | BSD-3-Clause |
| SemanticDiff | <https://semanticdiff.com>         | -                                           | Best        | Slow     | See pricing | -            |

## Conflict resolution

| Name       | Homepage                            | Repository                               | Performance | Speed    | Price | License |
| ---------- | ----------------------------------- | ---------------------------------------- | ----------- | -------- | ----- | ------- |
| diff3      | <https://git-scm.com>               | -                                        | -           | Moderate | Free  | -       |
| git-imerge | -                                   | <https://github.com/mhagger/git-imerge>  | -           | Slow     | Free  | GPL-2.0 |
| kdiff3     | <https://invent.kde.org/sdk/kdiff3> | <https://github.com/KDE/kdiff3>          | -           | Fast     | Free  | GPL-2.0 |
| Meld       | -                                   | <https://gitlab.gnome.org/GNOME/meld>    | -           | Moderate | Free  | GPL-2.0 |
| Mergiraf   | <https://mergiraf.org>              | <https://codeberg.org/mergiraf/mergiraf> | Best        | Fastest  | Free  | GPL-3.0 |
| zdiff3     | <https://git-scm.com>               | -                                        | Good        | Moderate | Free  | -       |

## Merge

| Name       | Homepage               | Repository                               | Performance | Speed   | Price | License |
| ---------- | ---------------------- | ---------------------------------------- | ----------- | ------- | ----- | ------- |
| git-imerge | -                      | <https://github.com/mhagger/git-imerge>  | -           | Slow    | Free  | GPL-2.0 |
| Mergiraf   | <https://mergiraf.org> | <https://codeberg.org/mergiraf/mergiraf> | Best        | Fastest | Free  | GPL-3.0 |

## Conclusion

1. Follow [delta](https://dandavison.github.io/delta/configuration.html) guide
2. Follow [difftastic](https://difftastic.wilfred.me.uk/git.html#difftool) guide
3. Follow [mergiraf](https://mergiraf.org/usage.html) guide
4. Follow below change

`~/.gitconfig`

```diff
+ [merge]
-  conflictStyle = diff3
+  conflictStyle = zdiff3
```
