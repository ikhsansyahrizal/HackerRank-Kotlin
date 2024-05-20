#a very big sum 


import java.io.*
import java.math.*
import java.security.*
import java.text.*
import java.util.*
import java.util.concurrent.*
import java.util.function.*
import java.util.regex.*
import java.util.stream.*
import kotlin.collections.*
import kotlin.comparisons.*
import kotlin.io.*
import kotlin.jvm.*
import kotlin.jvm.functions.*
import kotlin.jvm.internal.*
import kotlin.ranges.*
import kotlin.sequences.*
import kotlin.text.*

/*
 * Complete the 'aVeryBigSum' function below.
 *
 * The function is expected to return a LONG_INTEGER.
 * The function accepts LONG_INTEGER_ARRAY ar as parameter.
 */

```kotlin
fun aVeryBigSum(ar: Array<Long>): Long {
    // Write your code here
    var result: Long = 0
    for (i in ar.indices) {
        result += ar.elementAt(i)
    }
    return result
}

fun main(args: Array<String>) {
    val arCount = readLine()!!.trim().toInt()

    val ar = readLine()!!.trimEnd().split(" ").map{ it.toLong() }.toTypedArray()

    val result = aVeryBigSum(ar)

    println(result)
}
```


<img width="800" alt="aVeryBigSum" src="https://github.com/ikhsansyahrizal/HackerRank-Kotlin/assets/72852911/31166465-36ba-421c-8cd1-2db80132847d">


