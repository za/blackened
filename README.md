A simple repo to demonstrate how we can run black before committing the changes.

```
(.venv) ➜  blackened git:(main) ✗ gc
[WARNING] The 'rev' field of repo 'https://github.com/psf/black' appears to be a mutable reference (moving tag / branch).  Mutable references are never updated after first install and are not supported.  See https://pre-commit.com/#using-the-latest-version-for-a-repository for more details.  Hint: `pre-commit autoupdate` often fixes this.
black....................................................................Failed
- hook id: black
- files were modified by this hook

reformatted hi.py

All done! ✨ 🍰 ✨
1 file reformatted.


diff --git a/hi.py b/hi.py
index a8e37b7..cfe2320 100644
--- a/hi.py
+++ b/hi.py
@@ -1,7 +1,8 @@
 #!/usr/bin/python3
 
-a= 3
-b= 4
+a = 3
+b = 4
 
-def hola(a,b):
-    print('hihihi ')
+
+def hola(a, b):
+    print("hihihi ")
```

Reference: https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/
