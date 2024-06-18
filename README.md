## Plus Minus

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
 * Complete the 'plusMinus' function below.
 *
 * The function accepts INTEGER_ARRAY arr as parameter.
 */
```kotlin
fun plusMinus(arr: Array<Int>): Unit {
    // Write your code here
    var zero = 0
    var plus = 0
    var minus = 0
    for(num in arr) {
        when {
            num == 0 -> zero++
            num < 0 -> minus++
            num > 0 -> plus++
        }
    }
    
    val plusRatio = plus.toDouble() / arr.size
    val minusRatio = minus.toDouble() / arr.size
    val zeroRatio = zero.toDouble() / arr.size
    
    println(String.format("%.6f", plusRatio))
    println(String.format("%.6f", minusRatio))
    println(String.format("%.6f", zeroRatio))
}

fun main(args: Array<String>) {
    val n = readLine()!!.trim().toInt()

    val arr = readLine()!!.trimEnd().split(" ").map{ it.toInt() }.toTypedArray()

    plusMinus(arr)
}
```

&nbsp;
&nbsp;


<img width="1000" alt="Screenshot 2024-06-18 at 20 05 22" src="https://github.com/ikhsansyahrizal/HackerRank-Kotlin/assets/72852911/603cbdcb-953c-4688-be48-bd46ff1c3529">





