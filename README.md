# tensor-networks-project-6-parallel-scaling-solved
**TO GET THIS SOLUTION VISIT:** [Tensor networks Project 6-Parallel scaling Solved](https://www.ankitcodinghub.com/product/parallel-scaling-of-tensor-networks-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;126147&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Tensor networks Project 6-Parallel scaling Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Analyse the parallel scaling of tensor networks, either for quantum circuits or for variational searches.

Running tensor network simulations on multiple processes is a challenging task. While the algorithm might be trivial to parallelize, one of the main features of TN algorithm is intrinsically serial: the isometry center. It is however possible to “mimic” the isometry center working with the so-called Vidal form of MPS. From now on, we will only work with MPS. However, all the properties of having an isometry center, such as the fact that an optimally-local approximation is also the globally optimal one, are gone. For this reason, every $L$ layers of the algorithm you need to reisometrize the tensor network. You have two possibilities:

1. Serial reisometrization. You start from right end of the chain. We right canonize the MPS in that process, communicate the boundaries to the next process, and right canonize that process. We iterate until we hit the left boundary.

2. Parallel isometrization [1]. We apply identity gates for $L’$ layers, where a layer is an application of 2-qubits identities on all even(odd) qubits. In this way the isometry is exactly recovered after $L’=n/2$, where $n$ is the number of qubits. But also $L'&lt;n/2$ might be good enough.

In this project, you will have to address the parallel scaling of the parallel MPS algorithm. With parallel scaling we denote the speedup of the parallel algorithm over the serial algorithm, that, for reasonable sizes of the system, should be $O(n)$.

Tasks

Test the parallel implementation of MPS quantum circuits using mpi4py up to 16 qubits. Use a bond dimension Ï‡ = 64. Use different types of circuits: construction of a GHZ state, brickwall random circuit in 1d. Are the results correct?

The MPS state needs to be reisometrized any L layers. After how many layers of the brickwall quantum circuit you need to reisometrize?

For which number of cycles the parallel reinstation of the isometry introduced in [7] is faster than the serial reinstanti- ation of the isometry? Test the parallel scaling of trotterized ising model evolution

Test the parallel scaling of a QFT algorithm
