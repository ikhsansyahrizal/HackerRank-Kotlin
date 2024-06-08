##Diagonal Differences

searching the differents value between 2 diagonal numbers, this one take some time, because it's use 2D array concept, and i've to learn back about it (it's been some time so i'm forget)

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
 * Complete the 'diagonalDifference' function below.
 *
 * The function is expected to return an INTEGER.
 * The function accepts 2D_INTEGER_ARRAY arr as parameter.
 */

```kotlin
fun diagonalDifference(arr: Array<Array<Int>>): Int {
    // Write your code here
     var d1 = 0
     var d2 = 0
     
     //[0][0] [1][1] [2][2]

     for( i in 0 until arr.size) {
         d1 += arr[i][i]
         d2 += arr[i][arr.size - 1 - i]
     }
     
     return Math.abs(d1-d2)
}

fun main(args: Array<String>) {
    val n = readLine()!!.trim().toInt()

    val arr = Array<Array<Int>>(n, { Array<Int>(n, { 0 }) })

    for (i in 0 until n) {
        arr[i] = readLine()!!.trimEnd().split(" ").map{ it.toInt() }.toTypedArray()
    }

    val result = diagonalDifference(arr)

    println(result)
}
```


<img width="1000" alt="diagonal-differences" src="https://github.com/ikhsansyahrizal/HackerRank-Kotlin/assets/72852911/3673b621-b55c-4bef-a46d-50b94ee35a04">
