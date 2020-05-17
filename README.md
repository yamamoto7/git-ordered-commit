## Git Ordered Merge

### $B35MW(B
Git$B$K$*$$$F!"%U%!%$%k$d%G%#%l%/%H%j$r(Bmerge$B$9$k=g=x7h$a$r2DG=$K$7$^$9!#(B
$B8=;EMM$G$O%j%b!<%H%j%]%8%H%j$+$i$N(Bmerge$B$N$_$r%+%P!<$7$F$$$^$9!#(B

### Useage

#### $B%3%^%s%I(B
git-ordered-merge$B$H$$$&%U%!%$%k$r(BPATH$B$NDL$C$F$$$k>l=j$KCV$/!"(B
$B$^$?$O(BPATH$B$rDL$9;v$K$h$C$F%3%^%s%I$r;HMQ$9$k$3$H$,$G$-$k$h$&$K$J$j$^$9!#(B
```
$ git ordered-merge <remote> <branch> 
```

#### $B=gHV$N7h$aJ}(B

merge$B$7$h$&$H$7$F$$$k%W%m%@%/%H%k!<%H$KF~$C$F$$$k!"(B.git$BFb$K@_Dj%U%!%$%k$rDI2C$9$k$3$H$G=g=x$r7h$a$k$3$H$,$G$-$^$9!#(B
`.git/info/checkout-order`$B$H$$$&%U%!%$%k$rDI2C$7$F$/$@$5$$!#(B

$BNc(B
.git/info/checkout-order
```
server/
assets/
client/
.
```

$B>e5-$NNc$O!">e$+$i=gHV$K(Bmerge$B$5$l$F:G=*E*$K(B`.`$B$K$h$C$F%+%l%s%H%G%#%l%/%H%jFb$N$9$Y$F$N%U%!%$%k$r(Bmerge$B$9$k5-=R$G$9!#(B
