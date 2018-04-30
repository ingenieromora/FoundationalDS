# Association, Causation, Confounding Factors and Randomization

References: https://www.inferentialthinking.com/chapters/02/causality-and-experiments.html



 In data science, many such studies involve observations on a group of individuals, a factor of interest called a *treatment*, and an *outcome* measured on each individual.

 In a study of whether chocolate is good for the health, the individuals would indeed be people, the treatment would be eating chocolate, and the outcome might be a measure of blood pressure.



The fundamental question is whether the treatment has an effect on the outcome. Any relation between the treatment and the outcome is called an **association**. If the treatment causes the outcome to occur, then the association is ***causal***.



The establishment of causality often takes place in two stages. First, an association is observed. Next, a more careful analysis leads to a decision about causality.



##Association

**Example:** London 1850. Cholera.

People tried to explain the cause of the disease.

**John Snow .** Anesthetist. Symptoms: noted that the cause was something that people eat and drink

​	He visualized the problem drawing a map and noted that dirty water was the cause.

​	*Where is the handle to this pump?*



## Causation



*"John Snow compared the death rate in the places where the two water companies served water. The two groups were similar except for the treatment. There were no other differences between two groups."*

Comparison is a fundamental techniques to stablish association and causation

1. **Treatment Group** (individuals who did received the treatment)
2. **Control Group** (individuals who did not receive the treatment)

Scientists use **comparison** to identify an association between a treatment and an outcome. They compare the outcomes of a group of individuals who got the treatment (the *treatment group*) to the outcomes of a group who did not (the *control group*). For example, researchers today might compare the average murder rate in states that have the death penalty with the average murder rate in states that don’t.

![1525127962059](C:\Users\leandro.mora\Projects\DSTraining\FoundationsOfDataScience\images\johnsnow)

The *death rate* of S&V is 10 times greater than the Lambeth company.

The key was not only the *death rate*, but as the *two groups were similar* apart from the treatment that they were served





## Confounding

If the treatment and control groups have **systematic differences other than the treatment**, then it might be difficult to identify causality.In an observational study, if the treatment and control groups differ in ways other than the treatment, it is difficult to make conclusions about causality.



Such differences are often present in **observational studies**



When they lead researches **astray**, they are called **confounding factors**

An underlying difference between the two groups (other than the treatment) is called a *confounding factor*, because it might confound you (that is, mess you up) when you try to reach a conclusion.

**Example: Coffee and lung cancer.** Studies in the 1960’s showed that coffee drinkers had higher rates of lung cancer than those who did not drink coffee. Because of this, some people identified coffee as a cause of lung cancer. But coffee does not cause lung cancer. The analysis contained a confounding factor – smoking. In those days, coffee drinkers were also likely to have been smokers, and smoking does cause lung cancer. Coffee drinking was associated with lung cancer, but it did not cause the disease.



## Randomize



**Randomize Controlled experiments**  

An excellent way to avoid confounding is to assign individuals to the treatment and control groups *at random*, and then administer the treatment to those who were assigned to the treatment group. Randomization keeps the two groups similar apart from the treatment.

You can account -mathematically- for variability in the assignment

In Data Science **Random <> Haphazard** : *The randomization must be done carefully*

The method of randomization can be as simple as tossing a coin. It may also be quite a bit more complex. But every method of randomization consists of a sequence of carefully defined steps that allow chances to be specified mathematically. This has two important consequences.

1. It allows us to account–mathematically–for the possibility that randomization produces treatment and control groups that are quite different from each other.
2. It allows us to make precise mathematical statements about differences between the treatment and control groups. This in turn helps us make justifiable conclusions about whether the treatment has any effect.



### Randomized Controlled experiments VS Observational Studies



In some situations it might not be possible to carry out a randomized controlled experiment, even when the aim is to investigate causality. For example, suppose you want to study the effects of alcohol consumption during pregnancy, and you randomly assign some pregnant women to your “alcohol” group. You should not expect cooperation from them if you present them with a drink. In such situations you will almost invariably be conducting an observational study, not an experiment. Be alert for confounding factors.