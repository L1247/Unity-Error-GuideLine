# Unity-Error-GuideLine
整理自己遇到Compile Error or Runtime Error

# Runtime
* FormatException: Index (zero based) must be greater than or equal to zero and less than the size of the argument list.
 使用 string.Format(format , arg1 , arg2) 時遇到的，如果Format是這樣的格式
 format = "{0} ,{1} ,{2}" ; 
 但Call Api的時候卻只有給兩個參數時，則執行到那一行的時候就會跳出錯誤、甚至不會有錯誤(也不繼續往下執行，卡在那一行)。
