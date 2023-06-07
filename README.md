# ODBenchmark

A library of benckmark code corresponding to the paper ***A Interdisciplinary Survey on Origin-destination Flows Modeling: Theory and Techniques***.

## OD Prediction

**Problem Definition.** *Given the regional urban characteristics of the city $\{ \mathbf{X}_r | r \in \mathcal{R} \}$ and observed OD flows $\{ f_{ij} | <r_i, r_j> \in \mathcal{X} \}$ between part of OD pairs $\mathcal{X}$ , construct a model to predict the remaining unknown OD flows $\{ f_{ij} | <r_i, r_j> \notin \mathcal{X} \}$.*



## OD Construction

**Definition of OD Matrix.** *The OD flows are organized in the form of an OD matrix $\mathbf{F}$ shown below,*
$$
    \mathbf{F} = 
    \begin{bmatrix} 
        f_{11} & f_{12} & ...    & f_{1N} \\ 
        f_{21} & f_{22} & ...    & f_{2N} \\
        \vdots & \vdots & \ddots & \vdots \\
        f_{N1} & f_{N2} & ...    & f_{NN}
    \end{bmatrix},
$$
*in which each element represents the flow $f_{ij}$ between a specific pair of regions. An OD matrix generally represents the mobility flow between all regions within an entire city.*

**Problem Definition.** *The OD construction problem aims to construct the complete OD matrix $\mathbf{F}$ for the city based on easily accessible information without any OD flow information available.*

## OD Estimation

**Problem Definition.** *Given a set of observed temporal traffic counts or other relevant observations $\mathcal{T} = \{ x_i^t | t=1,..,T \text{ and } i = 1,...,N \}$ collected at various locations $\{ l_i | i=1,...,N \}$ within a transportation network (such as road segments, intersections, or sensor-equipped locations), the objective is to infer the underlying OD flows $\{f^t_{ij}\}$, i.e., the number of trips between different origin and destination pairs, that generated the observed traffic pattern.*

## OD Forecasting

**Problem Definition.** *Given a historical dataset of OD flows $\{ f^t_{ij} | t= 1,2,...,k-1 \}$ over a certain period of time, the objective is to forecast the OD flows for future time periods $\{ 
f^t_{ij} | t=k,k+1,... \}$.*

