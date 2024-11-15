## 进击的菜鸟

#### 序章

######	2024年11月15日，一个平常的周末。我用刚学会的git咒语和vscode工具，在异空间创造了自己的一个小小世界。这个世界的未来会怎样？就让我们拭目以待吧……
```  git咒语：
git add .
git commit -m "注释信息"
git push origin master
```
######  vscode工具是一个奇妙的工具，它可以帮助我尽快地适应这个异空间，但它也总有一点自作聪明，向我提出各种建议。当然，这些建议只出现在我的视网膜中，由我的大脑决定是否采用。接下来，我使用了第二个咒语，在创造这个世界的同时，创造了另外一个镜像世界，这两个世界的差别在于：墙。墙是我所处的真实世界的一个保护罩，虽然意识可以随意穿越，但肉体受到其强大的保护。
```  git咒语：
git remote set-url --add origin https://gitee.com/yzrps/GoGoRookie.git
```

#### 建造html小屋(1)

######  在穿越到异空间后，我决定先搭建一个简单的html小屋，给这个世界增加一点色彩和元素。很久以前，我有过一个师傅，他最喜欢凭空造物，现在我决定试试他的魔法，凭空造出一个小屋来。这个小屋子的第一个能力是：可以使用css咒语检测自己的大小。
```css咒语：
@property --vw {
    syntax: '<length>';
    inherits: true;
    initial-value: 100vw;
}

@property --vh {
    syntax: '<length>';
    inherits: true;
    initial-value: 100vh;
}

:root {
    --w: tan(atan2(var(--vw), 1px));
    --h: tan(atan2(var(--vh), 1px));
}

body::before {
    content: counter(w) "x" counter(h);
    counter-reset: w var(--w) h var(--h);
    font-size: 150px;
    font-weight: 900;
    position: fixed;
    inset: 0;
    width: fit-content;
    height: fit-content;
    margin: auto;
}
```