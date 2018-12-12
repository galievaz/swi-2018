conflict changes
- keep both your change and this change

diff --git a/double_hash.rb b/double_hash.rb
index cd9d72c..cfa6db8 100644
--- a/double_hash.rb
+++ b/double_hash.rb
@@ -1,5 +1,4 @@
-h = {:bacon => 200, :coconut => 300}
-h.each { |k,v| h[k] = v*2 }
-
 # result is {:bacon=>400, :coconut=>600}
 
+h = {:bacon => 200, :coconut => 300}
+h.transform_values! { |v| v * 2 }
diff --git a/transform_values.patch b/transform_values.patch
index 8633859..e69de29 100644
--- a/transform_values.patch
+++ b/transform_values.patch
@@ -1,12 +0,0 @@
-diff --git a/double_hash.rb b/double_hash.rb
-index cd9d72c..cfa6db8 100644
---- a/double_hash.rb
-+++ b/double_hash.rb
-@@ -1,5 +1,4 @@
--h = {:bacon => 200, :coconut => 300}
--h.each { |k,v| h[k] = v*2 }
--
- # result is {:bacon=>400, :coconut=>600}

