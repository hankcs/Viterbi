Viterbi
========

An implementation of HMM-Viterbi Algorithm
----------------------

 - How to Use
 
```java
public static void main(String[] args)
{
     int[] result = Viterbi.compute(observations, states, start_probability, transititon_probability, emission_probability);
     for (int r : result)
     {
        System.out.print(Weather.values()[r] + " ");
     }
}
```
 - About the alorithm
 See [Wiki][1]

  [1]: https://en.wikipedia.org/wiki/Viterbi_algorithm#Example
  
  
Viterbi
========

通用维特比算法的Java实现
----------------------

 - 调用方法
 
```java
public static void main(String[] args)
{
     int[] result = Viterbi.compute(observations, states, start_probability, transititon_probability, emission_probability);
     for (int r : result)
     {
        System.out.print(Weather.values()[r] + " ");
     }
}
```
 - 算法详解
 代码本身没什么新意，看到Git上没有好用的Viterbi的Java实现，所以补个缺。特点是简单好懂，一个方法搞定。调用简单，往compute方法里填充HMM的五元组就能得到最佳标注序列。
 附赠一个对经典天气预测问题的求解，问题的描述和思路详见前文：
 详见[《HMM与分词、词性标注、命名实体识别》][2]

  [2]: http://www.hankcs.com/nlp/hmm-and-segmentation-tagging-named-entity-recognition.html