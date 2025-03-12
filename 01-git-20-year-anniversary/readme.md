
```shell
git show e83c5163316f89bfbde7d9ab23ca2e25604af290
```

```shell
commit e83c5163316f89bfbde7d9ab23ca2e25604af290
Author: Linus Torvalds <torvalds@linux-foundation.org>
Date:   Thu Apr 7 15:13:13 2005 -0700

    Initial revision of "git", the information manager from hell

diff --git a/Makefile b/Makefile
new file mode 100644
index 0000000000..a6bba79ba1
--- /dev/null
+++ b/Makefile
@@ -0,0 +1,40 @@
+CFLAGS=-g
+CC=gcc
+
+PROG=update-cache show-diff init-db write-tree read-tree commit-tree cat-file
+
+all: $(PROG)
+
+install: $(PROG)
+       install $(PROG) $(HOME)/bin/
+
+LIBS= -lssl
+
+init-db: init-db.o
+
:
```
