# Day-9-Recursion-3
Day 9: Recursion 3 app.patika.dev factorial function
<img width="936" alt="Ekran Resmi 2022-05-21 15 13 57" src="https://user-images.githubusercontent.com/105243448/169651040-9b369a2d-75fa-4a90-80f4-6b39b2d726ec.png">





```
using System.CodeDom.Compiler;
using System.Collections.Generic;
using System.Collections;
using System.ComponentModel;
using System.Diagnostics.CodeAnalysis;
using System.Globalization;
using System.IO;
using System.Linq;
using System.Reflection;
using System.Runtime.Serialization;
using System.Text.RegularExpressions;
using System.Text;
using System;

class Result
{

    /*
     * Complete the 'factorial function' below.
     *
     * The function is expected to return an INTEGER.
     * The function accepts INTEGER n as parameter.
     */

    public static int factorial(int n)
    {
        int result =1;
        for(int i=1; i<=n; i++){
            result *= i;
        }
        
        return result;
    }

}

class Solution
{
    public static void Main(string[] args)
    {
        TextWriter textWriter = new StreamWriter(@System.Environment.GetEnvironmentVariable("OUTPUT_PATH"), true);

        int n = Convert.ToInt32(Console.ReadLine().Trim());

        int result = Result.factorial(n);

        textWriter.WriteLine(result);

        textWriter.Flush();
        textWriter.Close();
    }
}


```
