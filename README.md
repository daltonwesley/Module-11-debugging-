# Module-11-debugging-
tukey_multiple &lt;- function(x) { outliers &lt;- array(TRUE,dim=dim(x)) for (j in 1:ncol(x)) {outliers[,j] &lt;- outliers[,j] &amp;&amp; tukey.outlier(x[,j])} outlier.vec &lt;- vector(length=nrow(x)) for (i in 1:nrow(x)) { outlier.vec[i] &lt;- all(outliers[i,])} return(outlier.vec) }
