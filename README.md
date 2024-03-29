# FNICM
FNICM is a tool to identify core nodes from significantly perturbed subnetwork.
If you used this tool, please cite our article: Li Q, Yin YH, Liu ZW, et al. FNICM: A New Methodology To Identify Core Metabolites Based on Significantly Perturbed Metabolic Subnetworks. Analytical Chemistry. 2024. doi: 10.1021/acs.analchem.3c04131.  

**Statement of Use**    
    The FNICM software is provided for research purposes only. For commercial use, please contact me at nikki77liqi@163.com.  

**Download**  
    Please click the link at https://github.com/LiQi94/FNICM/archive/refs/heads/main.zip to download the FNICM software and other files.  

**Usage**  
The software doesn’t require installation and simply double-click the ‘FNICM.exe’ to open it (Compatible exclusively with the Windows operating system). Then you can see the opened window in your desktop.   
![image](https://github.com/LiQi94/FNICM/blob/main/images/Figure1.png)  
 
Next, you can easily obtain the results after the following three steps.  
**1. Input file: digraph list**  
![image](https://github.com/LiQi94/FNICM/blob/main/images/Figure2.png)  
Here you need to input a digraph list file in a .txt format, which contains two columns of data, A and B. There is an edge from column A to column B. Note that this is an initial global network, and the subsequent subnetwork is constructed based on this network.  
![image](https://github.com/LiQi94/FNICM/blob/main/images/Figure3.png)  
 
**2. Input file: initial trust scores list**   
![image](https://github.com/LiQi94/FNICM/blob/main/images/Figure4.png)  
Here you need to set the initial trust scores of all nodes in the above digraph. Firstly, you need to select some nodes as seed nodes. Then according to your purpose of research, the initial scores can take a value between 0 and 1. Generally, the scores of seed nodes are set to 1, other remaining nodes are set to 0.  
![image](https://github.com/LiQi94/FNICM/blob/main/images/Figure5.png)  
 
**3. Set parameter: number of the top-rank nodes**  
Here you need to set the number of the top-ranked nodes you want to focus on based on your domain knowledge. Note that this number is closely related to the size of the constructed subnetwork. Then, you can click the ‘Start’ button to run the program.

**4. Output results**  
After the program finishes, you can obtain the following four files. These files are stored in the folder named Output_results within the directory where the software is saved.  
![image](https://github.com/LiQi94/FNICM/blob/main/images/Figure6.png)  
(1) TrustRank_scores: the list of the nodes in descending order with their scores.   
(2) Subnetwork_digraph: the digraph list of the constructed subnetwork.   
(3) Subnetwork_nodes: The ID list of all nodes in the above subnetwork.   
(4) Core_nodes: the list of core nodes identified from the above subnetwork using controllability analysis.  













