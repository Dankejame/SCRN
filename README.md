# SCRN
SCRN: Official implementation  of Single-cell Gene Regulatory Network Identification in Alzheimer's Disease.



## Installation and Running

Make sure the required dependencies are met, you can use pip or conda to install environment for SCRN：
1. Install [PyTorch](https://pytorch.org/).

2. please read [guide](./model/Python/README.md) for detail to install environment.

3. train:

     python -u Main.py --data-name xxx --hop  auto  --max-nodes-per-hop 200 --max-train-num 3000 --use-embedding  --use-attribute  --save-model 
4. predict:

    python Main.py  --data-name xxx   --hop auto --use-embedding  --use-attribute   --only-predict   --test-name  xxx  --max-nodes-per-hop  200

## Data 
GSE138852 :
    The initial gene expression matrix obtained by exper-iments has a total of 22,694 genes and 14,876 cells. As shown in the original work, low-quality genes and cells were filtered out, resulting in 10,850 genes and 13,214 cells, which include 2,171 astrocytes, 656 neurons, 449 microglia, 7,432 oligodendrocytes, 1,078 OPCs (oligodendrocyte progenitor cells), and 98 en-dothelial cells, respectively. All single-cell RNA se-quencing data are available from the Gene Expres-sion Omnibus (GEO) under the accession number GSE138852.

SYN18485175:
    The gene expression matrix of the microglia data has a total of 12,014 genes and 29,354 cells. As shown in the original work ,low-quality genes and cells were filtered out. The single-cell RNA sequencing data are available at Synapse (https://www.synapse.org/#!Synapse:syn18485175) under the doi 10.7303/syn18485175.

> The original document needs to be processed into the corresponding format to facilitate execution by Python. You may also modify the code as appropriate to match your target format.it required initialization files are located in the model/data path ([init file](https://drive.google.com/file/d/1Ukeaz6U7fYygOXeek6zkIxw9rUd71PTZ/view?usp=sharing)) and preprocessing related code will be updated later.