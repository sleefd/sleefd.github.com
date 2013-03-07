title: denclue review
footer: slee
subfooter: sleefd@gmail.come
gradient-colors: gray lime

density based clustering method:denclue
===


###agenda


* denclu idea 
* denclue advantage
* denclue definitions
* denclu algorithm


denclue idea
===

###Source


* influence function
describes the influence of data  


###method  

{% step %}
* overall density function  
sum of the influence function of all points
{% end %}
{% step %}
* density-attractors  
local maximal of density function  
hill climbing algorithm gudied by gradient
{% end %}
{% step %}
* clustering
{% end %}

denclue advantage
===
* arbitary shape clustering

* invariant against large amounts of noise

* work well for high dimensional data sets


denclue definitions
===
* influence function --->distance function

* gradient

* density attractor ---> local maximum

* outliers :  bound sigma

* Center-Defined cluster  
所有点都被中心点密度吸引

* Arbitary-Shape Cluster  
 >密度吸引， f >= sigma  
 >密度可达

denclue algorithm 
===
{% step %}
* 划分cube:边长 2delta
{% end %}
{% step %}
* 寻找high pupulated cubes  
    N >= SIGMA = sigma/2d
{% end %}

{%step%}
* 连接cube: dist(cube means) <= 4delta 
 {%end%}
{%step%}
* 爬山法寻找密度吸引子  
	爬山时同时记录与爬山路径距离较近的点
{%end%}
{%step%}
* 聚类
{%end%}
