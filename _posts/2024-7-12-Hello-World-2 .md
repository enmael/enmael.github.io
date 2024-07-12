---
layout: post
title: 알고리즘 문제-C# - 거품정렬(bubble sort) 
date : 2024-07-12
author : "enmael"
categories: blog
---
<h2> 거품정렬 </h2>

<span style="font-size: 15px;">
  (거품 정렬 알고리즘 설명)
</span>
<span style="font-size: 15px;">
  코드 
</span>
```csharp
int[] array = new int[5] { 32, 5, 7, 1, 27 };
int number = 0;

for(int i = 0; i < array.Length-1; i++) 
{
    for(int j = 0; j < (array.Length-i)-1; j++)
    {
        //if (j < array.Length - 1)
        //{
            if (array[j] > array[j+1])
            {
                number = array[j];
                array[j] = array[j+1];
                array[j + 1] = number;
            }
        //}
     
    }
}

for(int i =0; i < array.Length; i++)
{
    Console.Write(array[i]+ ", ");
}
```
<span style="font-size: 15px;">
  실행결과
</span>
![3]({{ site.baseurl }}/images/3.png)
