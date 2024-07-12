---
layout: post
title: 알고리즘 문제-C# - 에라토스의 채 
date : 2024-07-12
author : "enmael"
categories: blog
---
<h2> 에라토스의 채 </h2>

<span style="font-size: 15px;">
  (에라토스 채 설명 )
</span>

```csharp
int number = 100;
int[] array = new int[number]; 

for(int i = 0; i < number; i++)
{
    array[i] = i;
}

Sieve(array);

```

```csharp

static void Sieve(int[]x)
{

    for(int i =2; i<x.Length; i++)
    {
        
        if (x[i] != 2 && x[i]%2 ==0)
        {
            x[i] = 0;
        }
        else if(x[i] != 3 && x[i] % 3 == 0)
        {
            x[i] = 0;
        }
        else if (x[i] != 5 && x[i] % 5 == 0)
        {
            x[i] = 0;
        }
        else if (x[i] != 7 && x[i] % 7 == 0)
        {
            x[i] = 0;
        }
        
    }
}
```
```csharp

for (int i = 0; i < number; i++)
{
    
    Console.Write(array[i] + " ");
    if (i !=0 && i%10 == 0)
    {
        Console.WriteLine();
    }
}

Console.WriteLine();
Console.WriteLine();
Console.WriteLine(number +"까지의 소수는 :");
for (int i = 0; i < number; i++) 
{
    if (array[i] != 1 && array[i] != 0)
    {
        Console.Write(array[i]+", ");
    }
}
```

![2]({{ site.baseurl }}/images/2.PNG)
